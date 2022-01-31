@ECHO OFF
set errmsg="Missing_Files!"
if exist "%1phishinator.zip" GOTO error2

if not exist "phishinator1" set errmsg=%errmsg%+"phishinator1"
copy /b /v "phishinator1" "%1phishinator.zip"

if not exist "phishinator2" set errmsg=%errmsg%+"phishinator2"
copy /b /v "%1phishinator.zip"+"phishinator2" "%1phishinator.zip"

if not exist "phishinator3" set errmsg=%errmsg%+"phishinator3"
copy /b /v "%1phishinator.zip"+"phishinator3" "%1phishinator.zip"

if not exist "phishinator4" set errmsg=%errmsg%+"phishinator4"
copy /b /v "%1phishinator.zip"+"phishinator4" "%1phishinator.zip"

if %errmsg% == "Missing_Files!" GOTO good
ECHO %errmsg%
if exist "%1phishinator.zip" erase "%1phishinator.zip"
GOTO notfound
:good
ECHO Done, phishinator.zip restored.
GOTO end
:error
ECHO No file specified.
GOTO end
:error2
ECHO File phishinator.zip Already Exists.
GOTO end
:notfound
ECHO File(s) Missing. Restore ABORTED! 
GOTO end
:end
