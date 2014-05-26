skype-adfree
============

A registry key that disables ads on Skype for Windows. (Open with regedit)

##What it does

Adds apps.skype.com to Windows's internet exclusion zone 4 (Restricted) through the registry.

##Why not just block altogether it in hosts?

The problem is that Skype may use apps.skype.com for other purposes than ads.

Exclusion Zone 4 only prevents scripting and active content, which ads rely on.

##Reverting the changes

Delete 
```
    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Internet Settings\ZoneMap\Domains\skype.com 
```
through regedit.
