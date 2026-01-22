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
<img width="523" height="459" alt="imagen" src="https://github.com/user-attachments/assets/2ae0a356-2afa-4708-aeb2-e34e2d1710fe" />

2.- Sitúate en el directorio p1b. Crea los directorios (3_eval, teoriaa, teoriab) utilizando trayectorias relativas.
```
Set-Location C:\iso\p1b
New-Item -ItemType Directory -Name 3_eval
New-Item -ItemType Directory -Name teoriaa
New-Item -ItemType Directory -Name teoriab
```
<img width="523" height="254" alt="imagen" src="https://github.com/user-attachments/assets/f94862f1-406d-468a-88ef-a0ad131c3f1d" />

3.- Sitúate en el directorio iso. Crea el directorio (2_eval). 
```
cd C:\iso
mkdir 2_eval
```
<img width="523" height="254" alt="imagen" src="https://github.com/user-attachments/assets/cd0b8acd-b041-4a3e-ae8a-f019b22c0cbe" />

4.- Sitúate en el directorio 2_eval. Crea los directorios (prac1, prac2, prac3) con una única sentencia.
```
cd 2_eval
mkdir prac1
mkdir prac2
mkdir prac3
```
<img width="523" height="254" alt="imagen" src="https://github.com/user-attachments/assets/e2363392-27c6-44e8-8815-f67d0c23a313" />

5.- Sitúate en el directorio prac3. Crea los directorios (prac31, prac311) usando trayectorias relativas.
```
cd prac3
mkdir prac31
mkdir prac31\prac311
```
<img width="486" height="303" alt="imagen" src="https://github.com/user-attachments/assets/0b622152-32c7-4452-be22-2b7dabce04f4" />

6.- Accede al directorio iso usando trayectoria absoluta con una única sentencia.
```
cd C:\iso
```
<img width="277" height="55" alt="imagen" src="https://github.com/user-attachments/assets/c5dabd3a-5cb9-411d-a0fd-64e1a2708900" />

7.- Desde iso elimina los directorios (prac311, prac31,teoriab, teoriaa, t1, p1b, p1a) utilizando trayectorias absolutas. 
```
Remove-Item C:\iso\2_eval\prac3\prac31\prac311 -Recurse
Remove-Item C:\iso\2_eval\prac3\prac31 -Recurse
Remove-Item C:\iso\p1b\teoriab -Recurse
Remove-Item C:\iso\p1b\teoriaa -Recurse
Remove-Item C:\iso\t1 -Recurse
Remove-Item C:\iso\p1b -Recurse
Remove-Item C:\iso\p1a -Recurse
```
<img width="517" height="144" alt="imagen" src="https://github.com/user-attachments/assets/ab674adc-36ff-4f7b-a9b0-f0a3e482154f" />

8.- Accede al directorio 2_eval usando trayectoria relativa con una única sentencia.
```
cd 2_eval
```
<img width="517" height="144" alt="imagen" src="https://github.com/user-attachments/assets/50902fbb-87c1-4ad1-9b35-395557b6f7b7" />

9.- Desde aquí cambia el nombre del directorio prac1 por el de prac4.
```
Rename-Item prac1 prac4
```
<img width="517" height="183" alt="imagen" src="https://github.com/user-attachments/assets/644aeafc-da7a-46a8-b592-62a8a7ced7c8" />

10.- Desde aquí sitúa el directorio prac4 dentro del directorio prac3. 
```
Move-Item prac4 prac3
```
<img width="517" height="183" alt="imagen" src="https://github.com/user-attachments/assets/0e523473-4c7c-46fd-9f20-a4c6b7bacbd2" />

11.- Desde aquí elimina los directorios (1_eval, 3_eval)
```
Remove-Item C:\iso\1_eval
Remove-Item C:\iso\p1b\3_eval
```
<img width="369" height="43" alt="imagen" src="https://github.com/user-attachments/assets/52a8d193-e43d-4294-8cb0-d45f014274ed" />
12.- Ejecuta la orden para visualizar el árbol de directorios y subdirectorios dependientes del directorio iso
```
tree C:\iso /f
```
<img width="454" height="191" alt="imagen" src="https://github.com/user-attachments/assets/fdea3930-481b-4ecf-a8fc-dbbf5e55c980" />
13.- Accede directamente a la raíz (a la unidad en la que te encuentras)
```
cd \
```
<img width="454" height="191" alt="imagen" src="https://github.com/user-attachments/assets/a0f3d10e-c61b-4d9e-a119-515bcdccb801" />

