# LUDUS Templates

These directories are self-contained Ludus templates.

For more information see: https://docs.ludus.cloud/docs/templates

Here are some templates I'm using to get my ranges up.


## Easy template installation steps

1. Clone this repository

`git clone https://github.com/Croko-fr/ludus-templates.git`

2. Enter the directory

`cd ludus-templates`

3. Add the templates from directory

```bash
ludus templates add -d Debian/debian-10-10-x64-fr-server
ludus templates add -d Debian/debian-12-8-x64-fr-server
for filename in *-*; do ludus template add -d $filename; done;
```

4. Show templates list

```bash
ludus templates list
+----------------------------------------------------+-------+
|                      TEMPLATE                      | BUILT |
+----------------------------------------------------+-------+
| debian-10-10-x64-fr-server-template                | FALSE |
| debian-12-8-x64-fr-server-template                 | FALSE |
+----------------------------------------------------+-------+
```

5. Build the templates

```bash
ludus templates build -n debian-10-10-x64-fr-server-template
[INFO]  Template building started - this will take a while. Building 1 template(s) at a time.
```

6. Look at the install logs

```bash
ludus templates logs -f
```

7. After the building is succesfull

```bash
=>================
=> Build complete!
=>================
^C

ludus templates list
+----------------------------------------------------+-------+
|                      TEMPLATE                      | BUILT |
+----------------------------------------------------+-------+
| debian-10-10-x64-fr-server-template                | TRUE  |
| debian-12-8-x64-fr-server-template                 | FALSE |
+----------------------------------------------------+-------+
```

## BEEING TESTED

| OS type | Distribution | Version | Languages | Info |
|:---:|:---:|:---:|:---:|:---:|
| Microsoft | Windows Server | 2012 R2 | fr , us | |
| Linux | Kali | 2024.4 | fr , us | Desktop , Recon |
| Linux | Kali | 2024.4 | fr , us | Desktop , Web |

## TEMPLATES COVERAGE

### WINDOWS

| OS type | Distribution | Version | Languages | Info |
|:---:|:---:|:---:|:---:|:---:|
| Microsoft | Windows 10 | 21H2 LTSC | fr , us | |
| Microsoft | Windows 10 | 22H2 | fr , us | |
| Microsoft | Windows 11 | 22H2 | fr , us | |
| Microsoft | Windows 11 | 23H2 | fr , us | | 
| Microsoft | Windows Server | 2016 | fr , us | |
| Microsoft | Windows Server | 2019 | fr , us | |
| Microsoft | Windows Server | 2019 | fr , us | No security updates |
| Microsoft | Windows Server | 2022 | fr , us | |

### LINUX - ALMALINUX

| OS type | Distribution | Version | Languages |
|:---:|:---:|:---:|:---:|
| Linux | Almalinux | 8.10 | fr , us |
| Linux | Almalinux | 9.5 | fr , us |

### LINUX - DEBIAN

| OS type | Distribution | Version | Languages |
|:---:|:---:|:---:|:---:|
| Linux | Debian | 10.7 | fr , us |
| Linux | Debian | 10.8 | fr , us |
| Linux | Debian | 10.9 | fr , us |
| Linux | Debian | 10.10 | fr , us |
| Linux | Debian | 10.11 | fr , us |
| Linux | Debian | 10.12 | fr , us |
| Linux | Debian | 10.13 | fr , us |
| Linux | Debian | 11.0 | fr , us |
| Linux | Debian | 11.1 | fr , us |
| Linux | Debian | 11.2 | fr , us |
| Linux | Debian | 11.3 | fr , us |
| Linux | Debian | 11.4 | fr , us |
| Linux | Debian | 11.5 | fr , us |
| Linux | Debian | 11.6 | fr , us |
| Linux | Debian | 11.7 | fr , us |
| Linux | Debian | 11.8 | fr , us |
| Linux | Debian | 11.9 | fr , us |
| Linux | Debian | 11.10 | fr , us |
| Linux | Debian | 11.11 | fr , us |
| Linux | Debian | 12.0 | fr , us |
| Linux | Debian | 12.1 | fr , us |
| Linux | Debian | 12.2 | fr , us |
| Linux | Debian | 12.3 | fr , us |
| Linux | Debian | 12.4 | fr , us |
| Linux | Debian | 12.5 | fr , us |
| Linux | Debian | 12.6 | fr , us |
| Linux | Debian | 12.7 | fr , us |
| Linux | Debian | 12.8 | fr , us |
| Linux | Debian | 12.9 | fr , us |

### LINUX - KALI

| OS type | Distribution | Version | Languages | Packages |
|:---:|:---:|:---:|:---:|:---:|
| Linux | Kali | 2024.4 | fr , us | Desktop |
| Linux | Kali | 2024.4 | fr , us | Desktop , Pentest |

### LINUX - ROCKY

| OS type | Distribution | Version | Languages |
|:---:|:---:|:---:|:---:|
| Linux | Rocky | 8.10 | fr , us |
| Linux | Rocky | 9.5 | fr , us |

### LINUX - UBUNTU

| OS type | Distribution | Version | Languages |
|:---:|:---:|:---:|:---:|
| Linux | Ubuntu | 20.04.1 | fr , us |
| Linux | Ubuntu | 22.04.1 | fr , us |
| Linux | Ubuntu | 22.04.2 | fr , us |
| Linux | Ubuntu | 22.04.3 | fr , us |
| Linux | Ubuntu | 22.04.4 | fr , us |
| Linux | Ubuntu | 22.04.5 | fr , us |
| Linux | Ubuntu | 24.04.1 | fr , us |