1.- Situado en smm crea los directorios A, B, C y D. Utiliza trayectoria absoluta. 
```
mkdir C:\SMM\A
mkdir C:\SMM\B
mkdir C:\SMM\C
mkdir C:\SMM\D
```
<img width="409" height="301" alt="imagen" src="https://github.com/user-attachments/assets/bc2413d7-0daa-48d4-bb26-27cc8175feb8" />

2.- Sitúate en D y desde allí crea A1, A2, A21, A22, A221 con una única sentencia utilizando trayectoria relativa.
```
cd C:\SMM\D
mkdir A1, A2, A21, A22, A221
```

<img width="409" height="301" alt="imagen" src="https://github.com/user-attachments/assets/479ccaf1-058b-424b-9ab3-f2610844db2f" />

3.- Sitúate en A221 y desde allí crea B1, B11, B111, B112 con una única sentencia y utilizando trayectoria relativa.
```
cd A221
mkdir B1, B11, B111, B112
```
<img width="409" height="301" alt="imagen" src="https://github.com/user-attachments/assets/12a1987f-50e8-4a3c-84ff-a7b9bc3441dd" />

4.- Estando situado en A221, crea un fichero llamado líneas.txt en el directorio C que contenga el árbol de directorios dependiente del directorio A (incluyendo los subdirectorios). 
```
tree C:\SMM\A /f > C:\SMM\C\lineas.txt
```
<img width="409" height="74" alt="imagen" src="https://github.com/user-attachments/assets/9f735e74-e070-41d6-ae9e-01682334b223" />

5.- Crea en D un fichero llamado Nombre.txt que contenga tu nombre y otro fichero llamado Apellido.txt que contenga tu primer apellido.
```
echo TU_NOMBRE ILYA > C:\SMM\D\Nombre.txt
echo TU_APELLIDO STATOV > C:\SMM\D\Apellido.txt
```
<img width="409" height="74" alt="imagen" src="https://github.com/user-attachments/assets/c39f28ad-fdf4-4641-8198-6073bf7597b4" />

6.- Genera un fichero llamado union.txt en D que contenga nombre y tu primer apellido. 
```
type C:\SMM\D\Nombre.txt, C:\SMM\D\Apellido.txt > C:\SMM\D\union.txt
```
<img width="607" height="17" alt="imagen" src="https://github.com/user-attachments/assets/fea24ac6-746b-485a-92ef-5743e6489ef2" />

. 7.- Mueve el fichero union.txt a A21. 
```
move C:\SMM\D\union.txt C:\SMM\D\A21
```

<img width="607" height="17" alt="imagen" src="https://github.com/user-attachments/assets/2d889d74-1a36-43ad-b66f-e0cb42c0424e" />

8.- Mueve el directorio A2 dentro de C.
```
Move-Item C:\SMM\D\A2 C:\SMM\C
```
<img width="322" height="16" alt="imagen" src="https://github.com/user-attachments/assets/28ebcd77-f882-411a-aec1-9c0ab99da061" />

9.- Cambia el nombre del fichero union.txt por el de nuevaunion.txt 
```
Rename-Item C:\SMM\C\A2\A21\union.txt nuevaunion.txt
```
<img width="848" height="13" alt="imagen" src="https://github.com/user-attachments/assets/4458cb3c-1e06-4dc3-acf4-acee6167bcc6" />

10.- Copia el fichero Nombre.txt al directorio A.
```
Copy-Item C:\SMM\D\Nombre.txt C:\SMM\A
```
Copy-Item C:\SMM\D\Nombre.txt C:\SMM\A
```
<img width="848" height="13" alt="imagen" src="https://github.com/user-attachments/assets/ec7826ff-f1a6-4ed3-aa38-6e3e7882787f" />

11.- Elimina el directorio A (sin usar el parámetro /s).
```
Remove-Item C:\SMM\A
```
<img width="848" height="91" alt="imagen" src="https://github.com/user-attachments/assets/7cf9263e-faa3-4461-ab1a-be8856ac378d" />

12.- Cambia el nombre del fichero Apellido.txt por el de miApellido.doc
```
Rename-Item C:\SMM\D\Apellido.txt miApellido.doc
```
<img width="848" height="20" alt="imagen" src="https://github.com/user-attachments/assets/b3677c42-b86c-4ac6-95fb-2dfca9536977" />

13.- Cambia el nombre del directorio C por el de nuevoC
```
Rename-Item C:\SMM\C nuevoC
```
Rename-Item C:\SMM\C nuevoC
```
<img width="848" height="19" alt="imagen" src="https://github.com/user-attachments/assets/69a7aa09-0835-44fa-82ff-bfbc9b667c3b" />

14.- Copia el fichero lineas.txt a D con el nombre nlineasend.txt
```
Copy-Item C:\SMM\nuevoC\lineas.txt C:\SMM\D\nlineasend.txt
```
Copy-Item C:\SMM\nuevoC\lineas.txt C:\SMM\D\nlineasend.txt
```
<img width="587" height="20" alt="imagen" src="https://github.com/user-attachments/assets/c91a780e-2747-443f-968c-b971fbe94117" />
```
15.- Muestra el árbol de directorios (incluyendo ficheros) que depende del directorio smm.
```
tree C:\SMM /f
```
<img width="569" height="502" alt="imagen" src="https://github.com/user-attachments/assets/5174a370-1243-404d-be4e-bf79df57612e" />

