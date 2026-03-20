Windows Fundamentals Part 3:

Windows Security Update Guide: https://msrc.microsoft.com/update-guide (links the CVE database entries which is actually really helpful and cool - shows you what's been patched and what hasn't theoretically)

Why is it necessary sometimes to allow specific apps through the firewall?

Does modifying this setting to allow an app through participate in an attacker's toolkit?

I'm pretty sure firewall settings can also be modified from another configuration menu not just by going into advanced settings for firewalls using the settings menu.

More windows docs specifically for firewall best practices --> https://learn.microsoft.com/en-us/windows/security/operating-system-security/network-security/windows-firewall/configure (This would have been great for my Microsoft Server 2016 hardening/set up project at college.)

The exploit protection settings section is worth further research as it likely leads to studying a number of proven strategies that have been used with exploits in Windows, it's important to understand what each one is doing I feel.

I wonder if an exploit has ever been discovered for the TPM and if so how was it achieved reasonably since the claim that malicious software cannot tamper with it feels like a challenge I'm sure individuals have risen to the chance of trying to disprove. The physical security measures are definitely a good idea reasonably but I wonder again if those have been circumvented at any point. 

What is a crypto-processor, and how does it work? (ignoring the obvious autological answer)

BitLocker documentation by Microsoft --> https://learn.microsoft.com/en-us/windows/security/operating-system-security/data-protection/bitlocker/

Does the utility of BitLocker with TPM 1.2 or higher posit to get around known ransomware programs utilizing BitLocker to encrypt computer volumes for ransom?

The use of a startup key with bitlocker to prevent unauthorized access seems extremely secure and could potentially provide a great way of locking the computer down for someone attempting to hide something by simply destroying the drive the key is on. I wonder if there are forensics methods that get around this obvious way of locking information out from being seen especially when it locks down the start up process itself - does removing the key also shut the process down?

A little extension to working with VSS --> https://tryhackme.com/room/adventofcyber2

VSS is a back up feature that takes a snapshot of data but these snapshots tend to be deleted by malicious attackers using ransomware wherever possible. 

I saw there are VSS settings in the advanced systems settings earlier, I wouldn't experimenting with them. Also is there a way to protect the VSS snapshots from being deleted by attackers once the system has been compromised to the extent that ransomware is being used on it etc. 
Remote back ups do enable recovery from ransomware even if the shadow copies have been deleted but off site/remote backups aren't necessarily done frequently and significant data loss could still occur. 

Ooh there's some extra reading materials attached including something on "Living off the Land":

https://learn.microsoft.com/en-us/windows/win32/amsi/antimalware-scan-interface-portal
https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/configure?tabs=intune
https://support.microsoft.com/en-us/windows/configure-windows-hello-dae28983-8242-bb2a-d3d1-87c9d265a5f0#:~:text=Windows%2010,in%20with%20just%20your%20PIN.
https://www.csoonline.com/article/564531/the-best-new-windows-10-security-features.html
https://lolbas-project.github.io/#

I will probably attach sections for each of the further reading below.



