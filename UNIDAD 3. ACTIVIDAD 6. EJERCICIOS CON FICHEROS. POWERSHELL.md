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
