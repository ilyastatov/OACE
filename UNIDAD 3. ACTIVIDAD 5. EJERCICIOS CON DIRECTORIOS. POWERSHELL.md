# 0.- UNIDAD 3. ACTIVIDAD 5. EJERCICIOS CON DIRECTORIOS. POWERSHELL.
1.- Crea un directorio llamado iso en tu unidad c:. Sitúate en el directorio iso de tu unidad (que será la unidad C). Desde el directorio iso crea los directorios (1_eval, teoria, t1, practica, p1a, p1b) utilizando trayectorias absolutas. 
```
New-Item -ItemType Directory -Path C:\iso
Set-Location C:\iso

New-Item -ItemType Directory -Path C:\iso\1_eval
New-Item -ItemType Directory -Path C:\iso\teoria
New-Item -ItemType Directory -Path C:\iso\t1
New-Item -ItemType Directory -Path C:\iso\practica
New-Item -ItemType Directory -Path C:\iso\p1a
New-Item -ItemType Directory -Path C:\iso\p1b
```
