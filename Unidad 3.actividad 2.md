# 0.- Cambia el prompt a tu primera inicial del nombre y tu apellido
```
prompt Ilya $p^>
```
<img width="658" height="249" alt="image" src="https://github.com/user-attachments/assets/0576f8f5-0d42-4de0-9690-a6cab01b51b0" />

# 1.- Situado en smm crea los directorios A, B, C y D. Utiliza trayectoria absoluta.
```
md A,B,C,D
```
<img width="658" height="202" alt="image" src="https://github.com/user-attachments/assets/84dd7093-cd5a-40e0-8e1a-2a497d40e51b" />

# 2.- Sitúate en D y desde allí crea A1, A2, A21, A22, A221 con una única sentencia utilizando trayectoria relativa.
```
c:\smm>cd D

c:\smm\D>md ..\A\A1 ..\A\A2\ ..\A\A2\A21 ..\A\A2\A22\A2
```
<img width="658" height="157" alt="image" src="https://github.com/user-attachments/assets/ecee4c9b-1dda-4522-9240-7b3badc48289" />

# 3.- Sitúate en A221 y desde allí crea B1, B11, B111, B112 con una única sentencia y utilizando trayectoria relativa.
```
c:\smm>cd A\A2\A22\A221

c:\smm\A\A2\A22\A221>

c:\smm\A\A2\A22\A221>md ..\..\..\..\B\B1\B11\B111 ..\..\..\..\B\B1\B11\B112
```
<img width="658" height="221" alt="image" src="https://github.com/user-attachments/assets/15266cb2-7a0e-4021-9bcb-d1dd65f891ca" />

# 4.- Estando situado en A221, crea un fichero llamado líneas.txt en el directorio C que contenga el árbol de directorios dependiente del directorio A (incluyendo los subdirectorios).
```
C:\smm\A\A2\A22\A221>tree c:\smm\A > c:\smm\c\lineas.tx
```
<img width="658" height="58" alt="image" src="https://github.com/user-attachments/assets/6f341610-6518-4cc1-9007-ee4103936ee9" />

# 5.- Crea en D un fichero llamado Nombre.txt que contenga tu nombre y otro fichero llamado Apellido.txt que contenga tu primer apellido.
```
C:\smm\A\A2\A22\A221>echo Ilya > c:\smm\D\Nombre.txt

C:\smm\A\A2\A22\A221>echo Statov > c:\smm\D\Apellido.tx
```
<img width="658" height="96" alt="image" src="https://github.com/user-attachments/assets/62c6af6c-7d68-42d4-8736-0b45a759c456" />

# 6.- Genera un fichero llamado union.txt en D que contenga el contenido de Nombre.txt y Apellido.txt
```
C:\smm\D>type nombre.txt >> union.txt

C:\smm\D>type apellido.txt >> union.txt
```
<img width="658" height="98" alt="image" src="https://github.com/user-attachments/assets/c3f55691-8952-41be-8f30-c1aaaf4f3709" />

# 7.- Mueve el fichero union.txt a A21.
```
C:\smm\D>move union.txt ..\A\A2\A21
```
<img width="658" height="72" alt="image" src="https://github.com/user-attachments/assets/a9fb3012-01b5-4ed3-aa9d-8729a0a09ad4" />

# 8.- Mueve el directorio A2 dentro de C.
```
C:\smm\A>move A2 c:\smm\C
```
<img width="658" height="104" alt="image" src="https://github.com/user-attachments/assets/797db25d-1af2-4ec2-8957-eb362d5f4cb7" />

# 9.- Cambia el nombre del fichero union.txt por el de nuevaunion.txt
```
C:\smm\C\A2\A21>rename union.txt nuevaunion.txt
```
<img width="658" height="130" alt="image" src="https://github.com/user-attachments/assets/5414fae2-b705-4683-8e15-702026231ebc" />

# 10.- Copia el fichero Nombre.txt al directorio A.
```
C:\smm\D>copy Nombre.txt ..\A
```
<img width="658" height="110" alt="image" src="https://github.com/user-attachments/assets/14a4aec8-753f-4ed0-914d-cfabd137e774" />

# 11.- Elimina el directorio A (sin usar el parámetro /s).
```
C:\smm>erase A
```
<img width="658" height="71" alt="image" src="https://github.com/user-attachments/assets/e03d9e73-43b8-4632-917b-df1a14e1c0a1" />

# 12.- Cambia el nombre del fichero Apellido.txt por el de miApellido.doc
```
C:\smm\D>rename Apellido.txt Apellido.doc
```
<img width="658" height="55" alt="image" src="https://github.com/user-attachments/assets/1adbb7b3-74a1-46a2-8109-b93f67783f14" />

# 13.- Cambia el nombre del directorio C por el de nuevoC
```
C:\smm>rename C nuevoC
```
<img width="427" height="55" alt="image" src="https://github.com/user-attachments/assets/0dc450a7-f6ab-4e76-b5b7-1b4701432ea3" />

# 14.- Copia el fichero lineas.txt a D con el nombre nlineasend.txt
```
C:\>copy c:\smm\c\lineas.txt c:\smm\D\nuevolineas.tx
```
<img width="539" height="76" alt="image" src="https://github.com/user-attachments/assets/2c7b25e5-173d-45bf-b813-563ded457d20" />
