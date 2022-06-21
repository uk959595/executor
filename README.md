#superior eac/be injector pasta
#this shit was coded by me but i abandoned the future development actually
#maybe someone will find here something useful
#memory allocation method pasted from ThePerfectInjector and recoded to kernel with some additions like mdl allocation
#has custom cleaning shit and somewhat i think ud hook communication method

#https://github.com/estimated1337/exe...32a68d1985e316

#also some people may have problems with MEMORY_MANAGEMENT bsods
#that happens on some machines cuz of Spectre & Meltdown patches prevents exposing kernel memory to another process except current process context

#ONLY SUPPORT NOCRT DLLS WITHOUT IMPORTS

#fix is relatively easy, open command line as admin and type this:
#Code:
#reg add "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverride /t REG_DWORD /d 3 /f 
 
#reg add "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverrideMask /t REG_DWORD /d 3 /f
