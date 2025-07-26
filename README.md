# gitcoder_setup

mkdir ~/kiwispace

cd ./kiwispace

// Show file extensions Windows 10 powershell
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced" -Name "HideFileExt" -Value 0

Set-ExecutionPolicy -RemoteSigned Scope CurrentUser

//Present Working Directory $PWD
Invoke-WebRequest -Uri "https://repo.msys2.org/distrib/x86_64/msys2-base-x86_64-20250622.tar.xz" -OutFile "$PWD\msys2_installer.tar.xz"

Invoke-WebRequest -Uri "insertURI" -Outfile "$PWD\7zip_Portable"

Invoke-WebRequest -Uri "https://repo.msys2.org/distrib/x86_64/msys2-x86_64-20230718.exe" "$PWD\msys2_installer.exe

//sets up pacman on msys terminal
pacman -Syu

