# Insttal Laravel on docker using sail on Windows 10/11

1.Install WSL for windows
---------------------------------------------------------------------
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

2.Install Virtualmachine Platform
---------------------------------------------------------------------
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

3.Restart Windows

4.Install WSL2 Linux kernel update package for x64 machines :
---------------------------------------------------------------------
https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbGV6ZnI2QVFJemQzYWhOWnBUanpuQ0tDeEd2UXxBQ3Jtc0ttTXlnZmE1Nkt5bEdRcl9zR0JMTmRfczJ0a3FRYW5kX0h2NV9DeGZFSDFNa05hek0yRHY4eFpZZl9sUWJ4cUtaSWIwU0VuQ3FoUk5xVVpKYUxzNFN1MEkxUXg5clpUVTJjczN0RzhRenA5OW12TG9PMA&q=https%3A%2F%2Fwslstorestorage.blob.core.windows.net%2Fwslblob%2Fwsl_update_x64.msi&v=rr6AngDpgnM

5.Reset WSL as version 2
---------------------------------------------------------------------
wsl --set-default-version 2

6.Install Ubuntu from Windows Store

7.Run Ubuntu and setup user and password
8.Install Docker desktop
9.In docker setting General and Ressource : WSl intergration and enable Ubuntu

10.Install windows Terminal from Windows Store

11.on the command line : wsl
12.cd ~
13.Install Laravel
curl -s https://laravel.build/test-project | bash
14.in the browser bar :\\wsl$
move to you project folder to check
15. cd to the project directory
16. ./vendor/bin/sail up -d
17.Create alias
nano ~/.bashrc
++++
alias sail="bash vendor/bin/sail'
apply the changes : . ~/.bashrc
