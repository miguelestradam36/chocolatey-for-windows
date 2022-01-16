# Chocolatey Package Manager for Windows OS

![Chocolatey Logo](docs/Images/choco-logo.png "Chocolaye Logo")

## How to install ?

Step by step quick guide:

1. Search for Powershell
2. Open Powershell under administrative priviliges
3. Run the following command:
```bash
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
For more secure options direct to the [docs folder](docs/README.md)
 

### What is it ?

A Package Manager designed mainly for Windows Operating Systems.

Automate installs like GNU Make into Windows:
```bash
choco install make
```

Autromate installs like Visual Studio Code:
```bash
choco install vscode
```
With a single command.

### Functionalities

- [x] Package installations
- [x] Possibility of script automation
- [x] Simplify installations from commands/scripts

#### For more information

Please refer to: https://chocolatey.org/install