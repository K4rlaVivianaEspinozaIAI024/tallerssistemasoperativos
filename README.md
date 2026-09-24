# tallerssistemasoperativos
260301222
# Bitácora de Clase - Taller de Sistemas Operativos

**Matrícula:** 260301222  

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
