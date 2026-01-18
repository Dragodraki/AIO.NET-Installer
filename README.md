# AIO.NET-Installer
Installs/Repairs every relevant .NET application (Framework + Modern) from Windows 2000 onwards.
<br/>
(Release Date: 18.01.2026, Publisher: Dragodraki alias Dreamland, Notice: no fork)
<br/>

[<img src="https://user-images.githubusercontent.com/76787321/197257488-1b7aa8e9-9b6f-4600-949e-8ff477cb4bf4.png" width="23%"></img>](https://github.com/Dragodraki/AIO.NET-Installer/releases/latest/download/AIO.NETOfflineSetup.exe)
<br/>


-------------------------------
HOW IT WORKS TECHNICALLY
-------------------------------
Not much to say here - its my own app with distributing the neccessary versions of .NET Framework (v.1.0-4.8) and modern .NET Desktop Runtimes (v.5/6/7/8/9/10/...) in a single setup which was build with Inno Setup. The software iself is not special as it is/was officially available to download from Microsoft. The real magic is the configuration inside the installer which automatically detects your current Windows OS and offers the relevant and supported products only. Basically it's a ruleset I defined on my own based on my own knowledge about .NET support. Furthermore, the single products are called with special silent parameters to not disturb you while doing other stuff on your PC. If needed, you could even run the while EXE unatttended by starting with parameter "/VERYSILENT".

One more thing: .NET Framework 1.0 and 1.1 are not only out of date but also suffer from heavy security issues. That is why I strongly recommend against them and turned off the installation by default. Besides, they would create an entire additional user account "ASP.NET" for services which could be nasty to visit when clicking user profile options in start menu. If you still want .NET 1.0 and 1.1 being installed, you may to do so - you can savely delete this extra account "ASP.NET" afterwards (though .NET 1.0/1.1 might then cease to work correctly).
<br/>

To sum up: In theory, you can just blindly hit "Next" and then "Install" button in setup, without fiddling with the correct .NET version.

Here is a sample how it looks on  my german Windows 10 64-Bit:
<br/>
<img width="375" height="282" alt="AIO NET" src="https://github.com/user-attachments/assets/10e745fe-a5f5-402e-ae56-60ec12b08fa4" />

<br/>

-------------------------------
WINDOWS SUPPORT
-------------------------------
This setup was build to support all Windows OS beginning with Windows 2000.
The OS I actually tested the software are labeled with "---verified" at the end:

- Windows 2000 (---verified)
- Windows XP (---verified)
- Windows Server 2003
- Windows Vista
- Windows Server 2008 R1
- Windows 7 (---verified)
- Windows Server 2008 R2
- Windows 8/8.1
- Windows Server 2012 R1
- Windows Server 2012 R2
- Windows 10 (---verified)
- Windows Server 2016
- Windows Server 2019
- Windows 11 (---verified)
- Windows Server 2022
- Windows Server 2025
- ... probably next future Windows OS too
<br>


-------------------------------
LICENSE (OPEN-SOURCE)
-------------------------------
Permissions:
+ Private and Commcercial usage is allowed as long you don't demand money for it ;)
+ Forks are welcome, but they have to kept free of charge ;)
+ Free Distribution to friends or strangers is allowed, even wanted ;)

Limitations:
- Use the app at your own risk!
- Don't sell it as product as .NET is originally developed by Microsoft!
- Don't abuse it for malicious purposes!
<br/>

-------------------------------
USAGE
-------------------------------
Just open the EXE installer, optionally customize chosen .NET versions, hit "Next" and then "Install".<br/>
Depending on your OS and selections the install process will take from a few secconds to about 5 minutes.

If you want it to install unanttended with not even the wizard to be shown, call it with parameter "/VERYSILENT" and with these "/TASKS=":

repair - Fix general issues with NetFxRepairTool (Windows XP+) <br/>
net1_0 - Install .NET Framework 1.0 SP3 (known security issues; Windows 2000+) <br/>
net1_1 - Install .NET Framework 1.1 SP1 (known security issues; Windows 2000+) <br/>
net2_0 - Install .NET Framework 2.0 SP2 (Windows 2000/XP/Srv2003) <br/>
net3_5 - Install .NET Framework 3.5 (includes .NET 2.0+3.0; Windows XP+) <br/>
net4_0 - Install .NET Framework 4.0.3 (Windows XP) <br/>
net4_6 - Install .NET Framework 4.6 (Windows Vista/Srv2008R1) <br/>
net4_8 - Install .NET Framework 4.8 (Windows 7/Srv2008R2/8/Srv2012) <br/>
net4_8_1 - Install .NET Framework 4.8.1 (Windows 10 20H2+) <br/>
netc3_1 - Install .NET Core 3.1 (Windows 7+) <br/>
net5 - Install .NET Desktop Runtime 5.0.17 (Windows 7+) <br/>
net6 - Install .NET Desktop Runtime 6.0.36 (Windows 7+) <br/>
net7 - Install .NET Desktop Runtime 7.0.20 (Windows 7+) <br/>
net8 - Install .NET Desktop Runtime 8.0.22 (Windows 7+) <br/>
net9 - Install .NET Desktop Runtime 9.0.11 (Windows 7+) <br/>
net10 - Install .NET Desktop Runtime 10.0.1 (Windows 7+) <br/>
<br/>
If the site will be down far in the future, search the url with archive.org :)
<br/>
<br/>
