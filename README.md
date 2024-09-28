# office-project-rename
### blackpet ###
```
@echo off
setlocal enabledelayedexpansion

rem Set the search location and new file extension
set "DIR=I:\rename"
set "NEW=.blackpet"

rem Loop through all PDF files in the specified location
for /r "%DIR%" %%f in (*.pdf) do (
    set "filename=%%~nf"
    ren "%%f" "!filename!%NEW%"
)

echo All .pdf files have been renamed to %newExtension%
exit
```

### blackdog ###
```
@echo off
setlocal enabledelayedexpansion

rem Set the search location and new file extension
set "DIR=I:\rename"
set "NEW=.blackdog"

rem Loop through all PDF files in the specified location
for /r "%DIR%" %%f in (*.docx) do (
    set "filename=%%~nf"
    ren "%%f" "!filename!%NEW%"
)

echo All .pdf files have been renamed to %newExtension%
exit
```



### blackxxx ###
```
@echo off
setlocal enabledelayedexpansion

rem Set the search location and new file extension
set "DIR=I:\rename"
set "NEW=.blackxxx"

rem Loop through all PDF files in the specified location
for /r "%DIR%" %%f in (*.xlsx) do (
    set "filename=%%~nf"
    ren "%%f" "!filename!%NEW%"
)

echo All .pdf files have been renamed to %newExtension%
exit
```

### timmer ###
```
@echo off
rem Wait for 2 hours and 30 minutes (2.5 hours)
timeout /t 60

rem Run the .bat file located in I:\rename
call "I:\rename.bat"
setlocal

rem Get current time
set currentTime=%time%

rem Format the time to remove colons (:) for filename safety
set currentTime=%currentTime::=%

rem Create a text file with the current time
echo The current time is: %time% > "workdone_time_%currentTime%.txt"

endlocal
exit
```



