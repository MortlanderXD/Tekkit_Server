@ECHO OFF

:: When setting the memory below make sure to include the amount of ram letter. M = MB, G = GB.
set maxmemory=2G

:: Path to Java. Use full path like "C:\Program Files\Java\jdk1.7.0_80\bin\java.exe" or just "java" to use system default.
set "javapath=java"

:: Additional JVM arguments
set "jvmargs="

:: Pass-through args
set "launchargs=%*"

:: Handle ATLcustomjava override
IF "%1"=="ATLcustomjava" (
    shift
    set "javapath=%1"
    shift
    set "launchargs=%*"
    echo Using launcher-provided Java: %javapath%
)

:: Show Java info
echo.
echo Printing Java info below. If version doesn't appear, the Java path is wrong.
echo Java path: %javapath%
echo.

"%javapath%" -version
echo.

echo Launching minecraft_server.1.21.5.jar with %maxmemory% max memory
echo.

:: Launch server
"%javapath%" -Xmx%maxmemory% %jvmargs% -jar minecraft_server.1.21.5.jar %launchargs%

PAUSE
