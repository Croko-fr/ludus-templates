# LUDUS Templates

These directories are self-contained Ludus templates.

For more information see: https://docs.ludus.cloud/docs/templates

Here are some templates I'm using to get my ranges up.


## Easy template installation steps

1. Clone this repository

`git clone https://github.com/Croko-fr/ludus-templates.git`

2. Enter the directory

`cd ludus-templates`

3. Add the templates

```bash
ludus templates build -n almalinux-8-x64-fr-server-template
ludus templates build -n almalinux-9-x64-fr-server-template
for filename in *-*; do ludus template add -d $filename; done;
```

4. Build the templates

```bash
ludus templates build -n almalinux-8-x64-fr-server-template
[INFO]  Template building started - this will take a while. Building 1 template(s) at a time.
```

5. Look at the install logs

```bash
ludus templates logs -f
```