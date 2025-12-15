# Unidad 3. Actividad 1. Ejercicios con directivos


Actividad 1
```
cd / -> md iso -> cd iso -> md 1_eval -> cd 1_eval -> md teoria -> cd teoria -> md t1 -> cd .. -> md practica -> cd practica -> md p1a -> cd p1a -> md p1b
```
<img width="469" height="748" alt="image" src="https://github.com/user-attachments/assets/7ff66ab0-d525-45e8-a5e9-42f4c458bba5" />

#2 Sitúate en el directorio p1b. Crea los directorios (3_eval, teoriaa, teoriab) utilizando trayectorias relativas.

```
md..\..\..\..\3_eval\teoriaa ..\..\..\..\3_eval\teoriab
```
<img width="812" height="526" alt="image" src="https://github.com/user-attachments/assets/c9450b32-f859-47ff-a6e4-58a8605e38b5" />
#3 Sitúate en el directorio iso. Crea el directorio (2_eval).
```
cd C:\iso -> md 2_eval
```
<img width="812" height="526" alt="image" src="https://github.com/user-attachments/assets/fc7b9baa-d50c-4c0a-b529-32c45a1234df" />

#4 Sitúate en el directorio 2_eval. Crea los directorios (prac1, prac2, prac3) con una única sentencia.

```
cd C:\iso -> cd 2_eval -> md prac1 prac2 prac3
```
<img width="430" height="95" alt="image" src="https://github.com/user-attachments/assets/35549f14-fcea-4684-8a68-42b1f57b2958" />

5.- Sitúate en el directorio prac3. Crea los directorios (prac31, prac311) usando trayectorias relativas.
```
cd C:\iso -> cd 2_eval -> cd prac3 -> md prac31 prac311
```
6.- Accede al directorio iso usando trayectoria absoluta con una única sentencia.
```
C:\>cd c:\iso
```
<img width="144" height="78" alt="image" src="https://github.com/user-attachments/assets/de1caf47-4505-46a2-860e-737133712f6b" />
7.- Desde iso elimina los directorios (prac311, prac31,teoriab, teoriaa, t1, p1b, p1a) utilizando trayectorias absolutas.
```
c:\iso>rd /s c:\iso\1_eval\practica\p1a
c:\iso>rd /s c:\iso\3_eval\teoriaa
c:\iso\3_eval\teoriaa, ¿Está seguro (S/N)? S


c:\iso>rd /s c:\iso\3_eval\teoriab

c:\iso\3_eval\teoriab, ¿Está seguro (S/N)? S


c:\iso>rd /s c:\iso\1_eval\teoria\t1

c:\iso\1_eval\teoria\t1, ¿Está seguro (S/N)? S


c:\iso>rd /s c:\iso\2_eval\prac3\prac31

c:\iso\2_eval\prac3\prac31, ¿Está seguro (S/N)? S
```
<img width="478" height="836" alt="image" src="https://github.com/user-attachments/assets/2ba86156-d697-4bb0-8fb9-6474f63fad01" />
8.- Accede al directorio 2_eval usando trayectoria relativa con una única sentencia.
```
c:\iso\2_eval>
```
<img width="478" height="257" alt="image" src="https://github.com/user-attachments/assets/3424b8b9-380c-4592-9bb2-5b07796f9e87" />
9.- Desde aquí cambia el nombre del directorio prac1 por el de prac4.
```
c:\iso\2_eval>rename prac1 prac4
```
<img width="478" height="257" alt="image" src="https://github.com/user-attachments/assets/7265f44c-4e27-4f42-9990-fb52559c8d64" />
10.- Desde aquí sitúa el directorio prac4 dentro del directorio prac3.
```
c:\iso\2_eval>move prac2 prac4
```
<img width="478" height="212" alt="image" src="https://github.com/user-attachments/assets/2854efa7-175d-4ac3-8e72-d3619e3ab3df" />
11.- Desde aquí elimina los directorios (1_eval, 3_eval)
```
c:\iso\2_eval>rd /s /q c:\iso\1_eval ..\3_eval
```
<img width="478" height="544" alt="image" src="https://github.com/user-attachments/assets/5cf94e33-211e-43bf-a631-a6214068a2e9" />
12.- Ejecuta la orden para visualizar el árbol de directorios y subdirectorios dependientes del directorio iso
```
c:\iso\2_eval>tree c:\iso
```
<img width="478" height="176" alt="image" src="https://github.com/user-attachments/assets/2eeea3b6-08e0-49b7-aa4e-9ac9c5142492" />
13.- Accede directamente a la raíz (a la unidad en la que te encuentras)
```
c:\iso\2_eval>cd\
```
<img width="478" height="176" alt="image" src="https://github.com/user-attachments/assets/89613e70-3a00-4af0-9ddf-2d43f823a7c7" />
