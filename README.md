# StartAndStopAspCoreInWidowsAsService

ملف الأمر لإنشاء وتشغيل الخدمة (CreateAndStartService.bat):

set "projectPath=%~dp0"
sc create MyAspNetCoreService binPath= "%projectPath%YourProjectName.dll" start= auto
sc start MyAspNetCoreService
//-----------------------------------------------------------------
ملف الأمر لإيقاف الخدمة وحذفها (StopAndDeleteService.bat):
sc stop MyAspNetCoreService
sc delete MyAspNetCoreService
