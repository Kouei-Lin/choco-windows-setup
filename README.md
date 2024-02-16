# Choco Guide

Simple guide to setup apps quickly on Windows machine post installation via [chocolately](https://chocolatey.org/).

## Handy Choco Docs
- [Setup](https://docs.chocolatey.org/en-us/choco/setup)
- [Command](https://docs.chocolatey.org/en-us/choco/commands/)
- [Choco Packages](https://community.chocolatey.org/packages)

## Choco Install
Open Powershell as admin.

Run: `Get-ExecutionPolicy`. If it returns `Restricted`, then run: `Set-ExecutionPolicy AllSigned` or: `Set-ExecutionPolicy Bypass -Scope Process`.

Choco installation command: 

```Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))```

`choco -?` to check if choco is here.

`choco install googlechrome line adobereader anydesk.install` for essential apps. Adjust apps based on personal needs.

`choco list` to see installed apps.

`choco upgrade all` for upgrade.

`choco uninstall googlechrome` for uninstall. 
