# gitcoder_setup

mkdir ~/kiwispace

cd ./kiwispace

// Show file extensions Windows 10 powershell
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced" -Name "HideFileExt" -Value 0

Set-ExecutionPolicy -RemoteSigned Scope CurrentUser

Invoke-WebRequest -Uri "https://repo.msys2.org/distrib/msys2-i686-latest.sfx.exe" -OutFile "$PWD\msys2_installer.exe"
//Present Working Directory $PWD

