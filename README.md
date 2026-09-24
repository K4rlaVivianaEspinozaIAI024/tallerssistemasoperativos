# tallerssistemasoperativos
260301222
# Bitácora de Clase - Taller de Sistemas Operativos

# 🐧 Taller de Sistemas Operativos

**Estudiante:** Karla Viviana Espinoza Rubio  
**Matrícula:** 260301222  
**Institución:** Universidad / Taller de Sistemas Operativos  

---

## 📖 Introducción y Contexto Personal

Bienvenido a mi repositorio de la materia **Taller de Sistemas Operativos**. 

Este espacio funciona como mi **bitácora de clase**, donde documento el aprendizaje, comandos, conceptos teóricos y prácticas realizadas en la terminal de Linux durante el curso.

### Un tedioso Reto Académico
Adaptarme a esta asignatura ha representado un reto significativo y de gran crecimiento personal por dos razones clave:

1. **Brecha Académica (Gap Year):** Retomé mis estudios universitarios tras un periodo de algunos años fuera del entorno escolar desde que egresé de la preparatoria, por lo que retomar el ritmo de estudio, la lógica de trabajo y el estudio técnico requirió un esfuerzo de adaptación doble.
2. **Formación Previa Distinta:** En la educación media superior cursé la carrera técnica de **Laboratorista Clínico**, un área totalmente enfocada en las ciencias biológicas y de la salud, ajena al mundo de la informática, las ciencias de la computación o la administración de sistemas.

Afrontar por primera vez conceptos como la **interfaz de línea de comandos (CLI)**, **permisos octales**, **gestión de directorios en Linux** y el control de versiones con **Git y GitHub** implicó romper con mi zona de confort. Sin embargo, a través de la constancia, la toma detallada de apuntes y la práctica constante en laboratorio, he logrado construir una base sólida para entender el funcionamiento interno de los sistemas operativos.



---
---

## 📌 Bitácora de Clases

### 📅 Clase 1: 20 de Agosto de 2026
**Tema:** Navegación en el Sistema de Archivos y Control de Versiones

#### Estructura de Directorios en Linux
* `/`: Raíz del sistema de archivos.
* `/etc`: Archivos de configuración.
* `/home`: Carpeta de usuarios.
* `/root`: Cuenta del superusuario.
* `/var`, `/sys`, `/bin`, `/usr`, `/share`: Directorios del sistema.

#### Rutas Absolutas vs. Rutas Relativas
* **Ruta Absoluta:** Inicia desde la raíz `/` (ejemplo: `cd /etc/apt/services`).
* **Ruta Relativa:** Inicia desde el directorio actual (ejemplo: `cd ../user1`).

#### Comandos de Navegación
* `cd`: Cambia de directorio (`cd ~`, `cd $HOME` para ir a inicio).
* `find`: Busca archivos en el sistema.
* `printenv`: Muestra variables de entorno.
* `history`: Muestra el historial de comandos.

---

### 📅 Clase 2: 27 de Agosto de 2026
**Tema:** Banderas de `ls`, Operadores Lógicos y Redirección

#### Banderas del comando `ls`
* `ls -a`: Muestra archivos ocultos.
* `ls -lh`: Muestra el tamaño en formato legible para humanos (KB, MB).
* `ls -r`: Enlista en orden inverso.

#### Operadores Lógicos y Relacionales
* **Relacionales:** `>=`, `==`, `>`, `<=`, `<`, `!=`
* **Lógicos:** `AND` (&&), `OR` (||), `NOT` (!)
  * Ejemplo: `5 > 3 AND 2 == 2` $\rightarrow$ Verdadero (T)
  * Ejemplo: `2 > 1 OR 1 > 2` $\rightarrow$ Verdadero (T)

---

### 📅 Clase 3: 29 de Agosto de 2026
**Tema:** Introducción a la Interfaz de Usuario y Comandos Básicos

#### Conceptos Clave
* **GUI (Graphical User Interface):** Interfaz gráfica de usuario.
* **Comando:** Conjunto de instrucciones para el sistema.
* **Sintaxis:** Estructura correcta de un comando.

#### Comandos Básicos
* `help`: Muestra comandos disponibles.
* `touch`: Crea archivos vacíos (ejemplo: `touch uno.txt`).
* `ls`: Visualiza el contenido de un directorio.

> **Nota:** El sistema de archivos de Linux es *case-sensitive* (distingue entre mayúsculas y minúsculas).

---

### 📅 Clase 4: 15 de Septiembre de 2026
**Tema:** Permisos de Archivos en Linux

#### Estructura de Permisos (Octal)
* **4:** Lectura (`r`)
* **2:** Escritura (`w`)
* **1:** Ejecución (`x`)

Niveles: **Usuario / Grupo / Otros**

#### Ejemplos con `chmod`
* `chmod 400 file.txt`: Solo el propietario puede leer.
* `chmod 444 file.txt`: Todos pueden leer.
* `chmod 700 file.txt`: Acceso total solo para el propietario.
* `chmod +x file.txt`: Agrega permisos de ejecución.
* `chmod -wx file.txt`: Quita permisos de escritura y ejecución.
* `chown`: Cambia el propietario/grupo de un archivo.

---

### 📅 Clase 5: 17 de Septiembre de 2026
**Tema:** Caracteres Comodín (Wildcards) y Tuberías (`|`)

#### Comodines
* `*`: Representa cero o infinitos caracteres (ejemplo: `*.txt`, `s*`).
* `?`: Representa exactamente un carácter.

#### Comandos y Redirección
* `grep`: Filtra y busca texto.
* `|` (Pipe): Redirige la salida de un comando a la entrada de otro (ejemplo: `ls -1 | grep *.txt`).
* `>`: Redirige la salida a un archivo (ejemplo: `echo "Hola" > file.txt`).
* `date`: Muestra/manipula la fecha del sistema.
* `mkdir /tmp/taller`: Crea un directorio temporal.

---

### 📅 Práctica de Laboratorio (Secuencia de Comandos)

1. `cd /` — Ir a la raíz.
2. `cd $HOME` — Ir al directorio personal.
3. `ls` — Listar archivos.
4. `touch test.txt` — Crear archivo.
5. `cp test.txt test2.txt` — Copiar archivo.
6. `mv test2.txt test3.txt` — Renombrar/mover archivo.
7. `rm test2.txt` — Eliminar archivo.
8. `mkdir prueba` — Crear carpeta.
9. `mv test3.txt prueba/` — Mover archivo a carpeta.
10. `cp -r /home/prueba /home/prueba2/` — Copiar carpeta recursivamente.
11. `rm -rf prueba` — Eliminar carpeta de forma forzada.
12. `vi test3.txt` / `vi test4.txt` — Editar archivos con Vi.
13. `cat test3.txt test4.txt > test5.txt` — Concatenar archivos.
14. `clear` — Limpiar pantalla.
15. `whoami` — Mostrar usuario actual.
16. `history` — Ver historial de comandos.
----
### 📅 TAREA 997: maquina virtual con Linux

**Descripción:** Ejercicio práctico realizado en la terminal de Linux consistente en la ejecución secuencial de 22 comandos para la gestión de archivos, navegación de directorios, edición de texto y consulta del sistema.

#### 📝 Comandos Ejecutados

```bash
cd /
cd $HOME
pwd
ls
touch test.txt
cp test.txt test2.txt
mv test2.txt test3.txt
rm test2.txt
mkdir prueba
mv test3.txt prueba/
cp -r prueba prueba2
rm -rf prueba
mv test.txt prueba2/
cd prueba2
echo "Hola " > test3.txt
echo "Mundo" > test4.txt
cat test3.txt test4.txt > test5.txt
clear
whoami
cat test3.txt
netstat --help
history
---
GALERIA 997
---

### 🖼️ GALERIA 997

![prueba](https://github.com/user-attachments/assets/20a831a2-c4f6-40cc-a795-7f79b6fdc1c6)

![prueba2](https://github.com/user-attachments/assets/821eb202-66e8-4ea3-a4a2-fea7dece377b)

![prueba4](https://github.com/user-attachments/assets/7a5966c6-ac8a-46e3-b5a1-efb4cefb4266)

![prueba3](https://github.com/user-attachments/assets/932c26c3-cfd5-414c-bf77-865a8d320153)
