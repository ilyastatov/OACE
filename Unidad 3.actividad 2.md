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
