# Chocolatey quick tip

## How to

### Open Powershell under administrative priviliges

In case you are having problems doing the following task, please direct to: [Powershell: How to run as administrator from GUI](Powershell.md)

## Security

### More secure request
Using **AllSigned** insted of **ByPass**:
```bash
Set-ExecutionPolicy AllSigned -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

#### If your OS has resctrictions upon the execution

**First**

Please verify that state of the execution
```bash
Run Get-ExecutionPolicy. 
```
If it returns *Restricted*, then run one of the commands, depending on the type of execution you want to run:

```bash
Set-ExecutionPolicy AllSigned
```
or 
```bash
Set-ExecutionPolicy Bypass -Scope Process.
```