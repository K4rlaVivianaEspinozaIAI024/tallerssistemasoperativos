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
```
---
---

### 🖼️ GALERIA 997

![prueba](https://github.com/user-attachments/assets/20a831a2-c4f6-40cc-a795-7f79b6fdc1c6)

![prueba2](https://github.com/user-attachments/assets/821eb202-66e8-4ea3-a4a2-fea7dece377b)

![prueba4](https://github.com/user-attachments/assets/7a5966c6-ac8a-46e3-b5a1-efb4cefb4266)
---
---

### 📅 Tarea #995: Práctica e Introducción a Vim (`Vim Adventures`)

**Descripción:** Ejercicio de aprendizaje interactivo utilizando el entorno de *Vim Adventures* para dominar la navegación y comandos avanzados de movimiento en el editor de texto `vi` / `vim`.

#### 🎯 Aprendizajes Clave
* **Navegación Básica:** Uso de las teclas `h`, `j`, `k`, `l` para el desplazamiento de cursor.
* **Movimiento por Palabras:** 
  * `w`: Avanza al inicio de la siguiente palabra (*word*).
  * `b`: Retrocede al inicio de la palabra anterior (*word*).
* **Diferencia Crítica entre `word` y `WORD`:**
  * Las palabras en minúscula (`w`, `b`) consideran los signos de puntuación y caracteres especiales como delimitadores.
  * Las palabras en mayúscula (`W`, `B`) consideran como delimitador únicamente los espacios en blanco, permitiendo saltar bloques completos de texto y obstáculos (como el paso de las rocas hacia los cofres).

#### 📸 Evidencias de Progreso

![Evidencia Vim Adventures]

<img width="774" height="506" alt="bim1" src="https://github.com/user-attachments/assets/ab643e18-cd98-46c1-88d4-b601be023532" />

---

---

### 📅 Tarea #993: Creación de Menú Interactivo y Scripts en Bash

**Descripción:** Desarrollo de un script en Bash que despliega un menú de opciones para ejecutar de forma organizada la creación de un árbol de directorios, un script clásico de "Hola Mundo", un saludo interactivo con variables del sistema y la opción de salida.

#### 💻 Código del Script (`menu.sh`)

```bash
#!/bin/bash

# Muestra del menú principal de opciones
echo "=========================================="
echo "         MENÚ DE OPCIONES BASH            "
echo "=========================================="
echo "1) Crear árbol de directorios"
echo "2) Ejecutar script 'Hola Mundo'"
echo "3) Ejecutar script de Saludo (con variables)"
echo "4) Salir"
echo "=========================================="

# Evaluación de la opción seleccionada mediante la estructura 'case'
case $opcion in
    1)
        echo "--- Creando árbol de directorios ---"
        mkdir -p proyecto/{src,bin,docs,tests}
        echo "¡Estructura de directorios creada con éxito!"
        ls -R proyecto
        ;;
    2)
        echo "--- Ejecutando Hola Mundo ---"
        echo "Hola Mundo"
        ;;
    3)
        echo "--- Script de Saludo con Variables ---"
        nombre="Estudiante"
        usuario_sistema=$(whoami)
        fecha_actual=$(date +%D)
        
        echo "¡Hola, $nombre!"
        echo "Estás conectado como el usuario: $usuario_sistema"
        echo "La fecha de hoy es: $fecha_actual"
        ;;
    4)
        echo "Saliendo del menú... ¡Hasta luego!"
        ;;
    *)
        echo "Opción no válida."
        ;;
esac
```


https://github.com/user-attachments/assets/61400caf-38d3-4ebb-ac62-7b10360cd80d


---

### 📅 Tarea #992: Scripts en Bash

**Descripción:** Desarrollo de un script en Bash

#1
<img width="1184" height="771" alt="image" src="https://github.com/user-attachments/assets/2a08c6b2-cea3-4257-8dcd-ed1b37b95b95" />
2
<img width="1128" height="831" alt="image" src="https://github.com/user-attachments/assets/eb74675d-06e7-4d94-94ee-7be6f415c1de" />
3
<img width="1120" height="811" alt="image" src="https://github.com/user-attachments/assets/e8f57135-7a2f-4303-837d-fdff9beac242" />

4
<img width="1086" height="856" alt="image" src="https://github.com/user-attachments/assets/f8e4cf89-275c-48eb-8cf1-70ac52db245b" />

5
<img width="1081" height="792" alt="image" src="https://github.com/user-attachments/assets/9956ea4b-482f-4ad9-b7e8-5180d79a5f6f" />

6

<img width="792" height="828" alt="image" src="https://github.com/user-attachments/assets/02d5cb8b-7534-493e-bf58-0c77d5dee65f" />

7
<img width="829" height="717" alt="image" src="https://github.com/user-attachments/assets/071aff3f-5682-42ce-909d-996436781bd5" />



8

<img width="814" height="623" alt="image" src="https://github.com/user-attachments/assets/25c49f30-fdd9-45da-a25f-474ae81cb659" />


9

<img width="903" height="740" alt="image" src="https://github.com/user-attachments/assets/e24614a8-6568-47f1-8cf8-5ce1845268ef" />


10

<img width="582" height="421" alt="image" src="https://github.com/user-attachments/assets/5dae08f0-4b63-4f97-b16d-84d1a53ee857" />


11

<img width="732" height="753" alt="image" src="https://github.com/user-attachments/assets/a4596375-7097-4ba0-ac77-627577dff520" />
<img width="620" height="695" alt="image" src="https://github.com/user-attachments/assets/351196de-e74d-4895-8d5b-c9a1d40597ff" />
<img width="486" height="597" alt="image" src="https://github.com/user-attachments/assets/3d411bcd-f706-43db-bb66-ef349a399555" />



12

<img width="903" height="653" alt="image" src="https://github.com/user-attachments/assets/c75abe40-333f-4550-816b-985628e050bd" />


13

<img width="911" height="736" alt="image" src="https://github.com/user-attachments/assets/e9ee32a6-a29b-4e6b-bf16-5ffdedffd2da" />


14

<img width="910" height="661" alt="image" src="https://github.com/user-attachments/assets/60e55051-5a97-4215-97c0-3a1ea755bc71" />
<img width="669" height="633" alt="image" src="https://github.com/user-attachments/assets/62a6864b-da76-44a8-ac78-1b584bcbd854" />


15

<img width="611" height="742" alt="image" src="https://github.com/user-attachments/assets/58a37411-961c-4890-a22b-74694f14951f" />


16

<img width="805" height="627" alt="image" src="https://github.com/user-attachments/assets/ae8d6cf8-2f45-420b-87c9-68bac251eeba" />


17

<img width="683" height="573" alt="image" src="https://github.com/user-attachments/assets/e749a87c-96af-4906-8935-d1986c04f808" />


18

<img width="971" height="856" alt="image" src="https://github.com/user-attachments/assets/d7f69918-e654-4c05-8d01-c35b1dc0872d" />

----
### 📅 TAREA 994: Instalar Virtualbox y alguna distribucion de Linux,

<img width="1855" height="802" alt="image" src="https://github.com/user-attachments/assets/9e058e37-c315-4f0e-848c-e71dc952a559" />


