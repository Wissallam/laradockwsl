# Insttal Laravel on docker using sail on Windows 10/11

### 1.Install WSL for windows

> dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

### 2.Install Virtualmachine Platform

> dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

### 3.Restart Windows

### 4.Install WSL2 Linux kernel update package for x64 machines :
> https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi

### 5.Reset WSL as version 2

>wsl --set-default-version 2

### 6.Install Ubuntu from Windows Store

### 7.Run Ubuntu and setup user and password 
### 8.Install Docker desktop 
### 9.In docker setting General and Ressource : WSl intergration and enable Ubuntu

### 10.Install windows Terminal from Windows Store

### 11.on the command line :
> wsl 
### 12.
>cd ~ 
### 13.Install Laravel 
>curl -s  https://laravel.build/test-project  | bash 
### 14.in the browser bar :\wsl$ move to you project folder to check 
### 15. cd to the project directory 
### 16. 
>./vendor/bin/sail up -d 
### 17.Create alias 
>nano ~/.bashrc

Add the at the end of file :
> alias sail="bash vendor/bin/sail' 
> 
Apply the changes : 
>. ~/.bashrc
