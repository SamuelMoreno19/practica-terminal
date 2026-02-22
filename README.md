# practica-terminal
# Ejercicio practico - leccion #1
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir proyecto_final
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd  proyecto_final
@SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ mkdir codigo documentacion recursos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ touch codigo/main.py codigo/config.json
@SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ touch documentacion/README.md
@SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ tree proyecto_final
proyecto_final  [error opening dir]

0 directories, 0 files

@SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ cd ..
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree proyecto_final
proyecto_final
├── codigo
│   ├── config.json
│   └── main.py
├── documentacion
│   └── README.md
└── recursos

4 directories, 3 files
---------------------------------------------------

# Laboratorio 1: Archivo simple:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba.txt
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  proyecto_final  prueba.txt

# Laboratorio 2: Crear múltiples archivos:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo1.txt archivo2.txt archivo3.txt
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  archivo1.txt  archivo2.txt  archivo3.txt  proyecto_final  prueba.txt

# Laboratorio 3: Actualizar la marca de tiempo de un archivo:
touch prueba.txt
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:41 prueba.txt

# Laboratorio 4: Crear un directorio simple
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir documentos
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  archivo1.txt  archivo2.txt  archivo3.txt  documentos  proyecto_final  prueba.txt

# Laboratorio 5: Crear múltiples directorios
SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir fotos videos música
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md documentos fotos  música  proyecto_final videos

# Laboratorio 6: Crear directorios anidados
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p proyecto/src/main
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree proyecto
proyecto
└── src
    └── main
3 directories, 0 files

# Laboratorio 7: Combinar archivos y directorios
SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir trabajo
touch trabajo/informe.txt trabajo/notas.md
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls trabajo
informe.txt  notas.md

# Laboratorio 8: Crear una estructura compleja:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p biblioteca/{libros,revistas,artículos}
touch biblioteca/libros/novela.txt biblioteca/revistas/ciencia.md
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree biblioteca
biblioteca
├── artículos
├── libros
│   └── novela.txt
└── revistas
    └── ciencia.md
4 directories, 2 files

# Laboratorio 9: Proyecto final: 
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir mi_Proyecto
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd  mi_Proyecto
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ mkdir codigo documentacion recursos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ touch codigo/main.py codigo/config.json
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ touch documentacion/README.md
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ cd ..
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree mi_Proyecto
mi_Proyecto
├── codigo
│   ├── config.json
│   └── main.py
├── documentacion
│   └── README.md
└── recursos

4 directories, 3 files.

# Leccion 2 Navegación en el Sistema de Archivos con cd y pwd:
# Desafio final: 
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd /var/log
@SamuelMoreno19 ➜ /var/log $ pwd
/var/log

@SamuelMoreno19 ➜ /var/log $ cd ..
@SamuelMoreno19 ➜ /var $ pwd
/var

@SamuelMoreno19 ➜ /var $ cd -
/var/log
@SamuelMoreno19 ➜ /var/log $ pwd
/var/log

@SamuelMoreno19 ➜ /var/log $ cd ~
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace

# Laboratorio 1: Comprender el Directorio Actual:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ pwd
/workspaces/practica-terminal.
La ruta /workspaces/practica-terminal se divide de la siguiente manera:
- /(Raíz): Es el directorio raíz del sistema de archivos de Linux. Todo comienza aquí.
- workspaces/: Es una carpeta de primer nivel dentro de la raíz, utilizada comúnmente en entornos como GitHub Codespaces para agrupar los proyectos.
- practica-terminal/: Es el nombre de tu repositorio o carpeta específica de trabajo. Es donde estás creando todos tus archivos y laboratorios.
- El pwd lo que nos ayuda es a que no nos sintamos perdidos en nuestros directorios y saber en donde estamos dentro de nuestra maquina 

# Laboratorio 2: Cambiar al Directorio Raíz:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd /
@SamuelMoreno19 ➜ / $ pwd
/
@SamuelMoreno19 ➜ / $ ls
bin                boot  etc  home  lib.usr-is-merged  lib64  mnt  proc  run   sbin.usr-is-merged  sys  usr  vscode
bin.usr-is-merged  dev   go   lib   lib32              media  opt  root  sbin  srv                 tmp  var  workspaces
- Y como podemos observar con el comando (ls) nos suelta 13 directorios principales al menos en mi maquina de trabajo.

# Laboratorio 3: Navegar a un Directorio Específico:
@SamuelMoreno19 ➜ / $ cd /home
@SamuelMoreno19 ➜ /home $ pwd
/home
@SamuelMoreno19 ➜ /home $ ls
codespace  vscode
@SamuelMoreno19 ➜ /home $ cd codespace
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace

# Laboratorio 4: Uso de Rutas Relativas:
@SamuelMoreno19 ➜ / $ pwd
/
@SamuelMoreno19 ➜ / $ cd /home/codespace
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
@SamuelMoreno19 ➜ ~ $ cd ../../workspaces/practica-terminal/documentos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ pwd
/workspaces/practica-terminal/documentos

# Laboratorio 5: Volver al Directorio Anterior:
SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd /tmp
@SamuelMoreno19 ➜ /tmp $ pwd
/tmp
@SamuelMoreno19 ➜ /tmp $ cd -
/workspaces/practica-terminal/documentos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd -
/tmp
@SamuelMoreno19 ➜ /tmp $ cd -
/workspaces/practica-terminal/documentos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd - 
/tmp

# Laboratorio 6: Ir al Directorio Personal:
@SamuelMoreno19 ➜ /tmp $ cd ~
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
@SamuelMoreno19 ➜ ~ $ touch prueba.txt
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
@SamuelMoreno19 ➜ ~ $ ls
java  nvm  prueba.txt

# Laboratorio 7: Subir un Nivel en el Sistema de Archivos:
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
@SamuelMoreno19 ➜ ~ $ cd ../..
@SamuelMoreno19 ➜ / $ pwd
/

# Laboratorio 8: Combinar Rutas Relativas y Absolutas:
@SamuelMoreno19 ➜ / $ cd /home
@SamuelMoreno19 ➜ /home $ pwd
/home
@SamuelMoreno19 ➜ /home $ cd codespace
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
@SamuelMoreno19 ➜ ~ $ cd /home
@SamuelMoreno19 ➜ /home $ pwd
/home
La gran diferencia:
- Ruta Absoluta: Es como la dirección de una casa con calle, carrera y número (ej. /home/codespace). Empieza siempre desde la raíz (/) y funciona sin importar dónde estés.
- Ruta Relativa: Es como decir "pasa a la habitación de al lado". Depende de dónde estés parado y no empieza con /.

# Laboratorio 9: Crear y Navegar a un Nuevo Directorio: 
@SamuelMoreno19 ➜ /home $ mkdir ~/pruebas
@SamuelMoreno19 ➜ /home $ cd  ~/pruebas
@SamuelMoreno19 ➜ ~/pruebas $ mkdir nivell
@SamuelMoreno19 ➜ ~/pruebas $ cd nivell
@SamuelMoreno19 ➜ ~/pruebas/nivell $ pwd
/home/codespace/pruebas/nivell
@SamuelMoreno19 ➜ ~/pruebas/nivell $ ls
@SamuelMoreno19 ➜ ~/pruebas/nivell $

# Laboratorio 10: Explorar Directorios Ocultos:
@SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
@SamuelMoreno19 ➜ ~ $ ls -a
.              .bash_logout  .conda   .dotnet     .jupyter  .minikube   .php      .rbenv  .vscode-remote  java        pruebas
..             .bashrc       .config  .gitconfig  .local    .nvs        .profile  .ruby   .zprofile       nvm
.bash_history  .cache        .docker  .hugo       .maven    .oh-my-zsh  .python   .rvmrc  .zshrc          prueba.txt
@SamuelMoreno19 ➜ ~ $ cd .config
@SamuelMoreno19 ➜ ~/.config $ pwd
/home/codespace/.config
Los directorios que comienzan con un punto (.) están ocultos por dos razones:
- Orden visual: Evitan llenar la carpeta personal de archivos que el usuario no usa diariamente.
- Seguridad: Protegen archivos de configuración críticos contra modificaciones accidentales que podrían afectar el funcionamiento del sistema o las aplicaciones.

# Leccion 3 # Listando Contenidos con `ls` y sus Opciones en Linux:
# Sección 4: Ejercicios Prácticos:
# Ejercicio 1: Explora tu directorio actual:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  archivo1.txt  archivo2.txt  archivo3.txt  biblioteca  documentos  fotos  mi_Proyecto  música  proyecto  proyecto_final  prueba.txt  trabajo  videos

# Ejercicio 2: Encuentra archivos ocultos:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git       archivo1.txt  archivo3.txt  documentos  mi_Proyecto  proyecto        prueba.txt  videos
..  README.md  archivo2.txt  biblioteca    fotos       música       proyecto_final  trabajo

# Ejercicio 3: Analiza los permisos:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
total 48
-rw-rw-rw-  1 codespace root      9935 Feb 22 18:20 README.md
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo3.txt
drwxrwxrwx+ 5 codespace codespace 4096 Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace 4096 Feb 21 23:42 documentos
drwxrwxrwx+ 2 codespace codespace 4096 Feb 21 23:44 fotos
drwxrwxrwx+ 5 codespace codespace 4096 Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 2 codespace codespace 4096 Feb 21 23:44 música
drwxrwxrwx+ 3 codespace codespace 4096 Feb 21 23:46 proyecto
drwxrwxrwx+ 5 codespace codespace 4096 Feb 21 23:27 proyecto_final
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:41 prueba.txt
drwxrwxrwx+ 2 codespace codespace 4096 Feb 21 23:47 trabajo
drwxrwxrwx+ 2 codespace codespace 4096 Feb 21 23:44 videos
- la D en diferentes archivos al inicio significa (Directory) o Directorio en español, o mejor conocido como una carpeta dentro de tu maquina de trabajo.

# Ejercicio 4: Combina opciones:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lah
total 60K
drwxrwxrwx+ 12 codespace root      4.0K Feb 21 23:49 .
drwxr-xrwx+  5 codespace root      4.0K Feb 21 23:26 ..
drwxrwxrwx+  8 codespace root      4.0K Feb 22 00:51 .git
-rw-rw-rw-   1 codespace root       11K Feb 22 18:22 README.md
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo3.txt
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:48 biblioteca
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:42 documentos
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 fotos
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:50 mi_Proyecto
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 música
drwxrwxrwx+  3 codespace codespace 4.0K Feb 21 23:46 proyecto
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:27 proyecto_final
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:41 prueba.txt
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:47 trabajo
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 videos

# Sección 5: Desafío Final:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir mi_practica
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd  mi_practica
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ touch archivo1.txt archivo2.txt 
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ mkdir carpeta1 carpeta2
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ ls -lah
total 16K
drwxrwxrwx+  4 codespace codespace 4.0K Feb 22 18:25 .
drwxrwxrwx+ 13 codespace root      4.0K Feb 22 18:24 ..
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:25 archivo1.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:25 archivo2.txt
drwxrwxrwx+  2 codespace codespace 4.0K Feb 22 18:25 carpeta1
drwxrwxrwx+  2 codespace codespace 4.0K Feb 22 18:25 carpeta2
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ ls -R
.:
archivo1.txt  archivo2.txt  carpeta1  carpeta2

./carpeta1:

./carpeta2:

# Laboratorio 1: Exploración Básica del Directorio Actual:
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ ls
archivo1.txt  archivo2.txt  carpeta1  carpeta2
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ cd carpeta1
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica/carpeta1 (main) $ ls
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica/carpeta1 (main)
- Aqui podemos ver que al ejecutar el comando (ls) aparecen 2 archivos .txt, y 2 directorios los cuales son carpeta 1 y 2
- Pregunta de Reflexión: ¿Qué sucede si ejecutas ls en un directorio vacío?
- Si yo entro a una carpeta que no tiene nada o directorio (como mi carpeta1) y escribo el comando ls, la terminal no me mostrará nada. Simplemente una nueva linea de terminal para seguir colocando nuevos comandos, como el directorio esta vacio

# Laboratorio 2: Descubriendo Archivos Ocultos:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git       archivo1.txt  archivo3.txt  documentos  mi_Proyecto  música    proyecto_final  trabajo
..  README.md  archivo2.txt  biblioteca    fotos       mi_practica  proyecto  prueba.txt      videos

@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch .mi_archivo_secreto
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git                 README.md     archivo2.txt  biblioteca  fotos        mi_practica  proyecto        prueba.txt  videos
..  .mi_archivo_secreto  archivo1.txt  archivo3.txt  documentos  mi_Proyecto  música       proyecto_final  trabajo
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md     archivo2.txt  biblioteca  fotos        mi_practica  proyecto        prueba.txt  videos
archivo1.txt  archivo3.txt  documentos  mi_Proyecto  música       proyecto_final  trabajo

- Respuesta a la Pregunta de Reflexión: ¿Por qué algunos archivos están ocultos por defecto?
- Limpieza Visual: Como ya vimos en mi salida de la terminal, tengo archivos como .git o .mi_archivo_secreto. Si todos los archivos de configuración (que suelen ser muchos) estuvieran visibles, me seria mucho mas dificil encontrar tus carpetas importantes.
- Seguridad (Evitar accidentes): Al estar ocultos, es menos probable que los borres o los cambies por error. Normalmente, los archivos ocultos son la "columna vertebral" de mis programas o de Git; si no los ves, no se pueden cambiar o dañar.

# Laboratorio 3: Entendiendo los Detalles con l:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba.txt
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
total 60
-rw-rw-rw-  1 codespace root      16714 Feb 22 18:38 README.md
-rw-rw-rw-  1 codespace codespace     0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace     0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace     0 Feb 21 23:40 archivo3.txt
drwxrwxrwx+ 5 codespace codespace  4096 Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace  4096 Feb 21 23:42 documentos
drwxrwxrwx+ 2 codespace codespace  4096 Feb 21 23:44 fotos
drwxrwxrwx+ 5 codespace codespace  4096 Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 4 codespace codespace  4096 Feb 22 18:25 mi_practica
drwxrwxrwx+ 2 codespace codespace  4096 Feb 21 23:44 música
drwxrwxrwx+ 3 codespace codespace  4096 Feb 21 23:46 proyecto
drwxrwxrwx+ 5 codespace codespace  4096 Feb 21 23:27 proyecto_final
-rw-rw-rw-  1 codespace codespace     0 Feb 22 18:39 prueba.txt
drwxrwxrwx+ 2 codespace codespace  4096 Feb 21 23:47 trabajo
drwxrwxrwx+ 2 codespace codespace  4096 Feb 21 23:44 videos

- Qué permisos tiene el archivo: Los permisos son -rw-rw-rw-: r (read): Lectura - w (write): Escritura.

- Como se repite tres veces, significa que el Dueño, el Grupo y Otros pueden leer y escribir en él. (El primer - indica que es un archivo regular, no un directorio).

¿Quién es el propietario?
- El propietario es codespace. (Es el primer nombre que aparece después del número 1). El segundo codespace es el grupo al que pertenece.

# Laboratorio 4: Formato Legible con lh:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lh
total 60K
-rw-rw-rw-  1 codespace root       17K Feb 22 18:42 README.md
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo3.txt
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:42 documentos
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:44 fotos
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 4 codespace codespace 4.0K Feb 22 18:25 mi_practica
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:44 música
drwxrwxrwx+ 3 codespace codespace 4.0K Feb 21 23:46 proyecto
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 21 23:27 proyecto_final
-rw-rw-rw-  1 codespace codespace    0 Feb 22 18:39 prueba.txt
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:47 trabajo
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:44 videos

@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ dd if=/dev/zero of=archivo_grande bs=1M count=10
10+0 records in
10+0 records out
10485760 bytes (10 MB, 10 MiB) copied, 0.00819897 s, 1.3 GB/s

# Pregunta de Reflexión: ¿Por qué es útil mostrar el tamaño en formato legible?
- Interpretación Rápida: No es lo mismo leer 1073741824 que leer 1G. El formato humano te permite saber al instante si un archivo es pesado o liviano sin tener que contar dígitos o hacer divisiones mentales.

Prevención de Errores: Al ver unidades como K (Kilobytes), M (Megabytes) o G (Gigabytes), puedes identificar rápidamente archivos que estén llenando el disco duro innecesariamente.

# Laboratorio 5: Ordenando por Tiempo de Modificación:
SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lt
total 10300
-rw-rw-rw-  1 codespace root         19035 Feb 22 18:45 README.md
-rw-rw-rw-  1 codespace codespace 10485760 Feb 22 18:42 archivo_grande
-rw-rw-rw-  1 codespace codespace        0 Feb 22 18:39 prueba.txt
drwxrwxrwx+ 4 codespace codespace     4096 Feb 22 18:25 mi_practica
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:47 trabajo
drwxrwxrwx+ 3 codespace codespace     4096 Feb 21 23:46 proyecto
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 fotos
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 música
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 videos
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:42 documentos
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo3.txt
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:27 proyecto_final

-  Modificando prueba.txt miremos que aparece como primer archivo al listar todos con el comando (ls -lt)
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lt
total 10300
-rw-rw-rw-  1 codespace codespace        0 Feb 22 18:46 prueba.txt - Aca esta
-rw-rw-rw-  1 codespace root         20183 Feb 22 18:46 README.md
-rw-rw-rw-  1 codespace codespace 10485760 Feb 22 18:42 archivo_grande
drwxrwxrwx+ 4 codespace codespace     4096 Feb 22 18:25 mi_practica
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:47 trabajo
drwxrwxrwx+ 3 codespace codespace     4096 Feb 21 23:46 proyecto
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 fotos
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 música
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 videos
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:42 documentos
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo3.txt
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:27 proyecto_final

# Laboratorio 6: Listado Recursivo con R:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p mi_directorio/subdirectorio1/subdirectorio2
touch mi_directorio/archivo1.txt
touch mi_directorio/subdirectorio1/archivo2.txt

@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -R
.:
README.md     archivo2.txt  archivo_grande  documentos  mi_Proyecto    mi_practica  proyecto        prueba.txt  videos
archivo1.txt  archivo3.txt  biblioteca      fotos       mi_directorio  música       proyecto_final  trabajo

./biblioteca:
artículos  libros  revistas

./biblioteca/artículos:

./biblioteca/libros:
novela.txt

./biblioteca/revistas:
ciencia.md

./documentos:

./fotos:

./mi_Proyecto:
codigo  documentacion  recursos

./mi_Proyecto/codigo:
config.json  main.py

./mi_Proyecto/documentacion:
README.md

./mi_Proyecto/recursos:

./mi_directorio:
archivo1.txt  subdirectorio1

./mi_directorio/subdirectorio1:
archivo2.txt  subdirectorio2

./mi_directorio/subdirectorio1/subdirectorio2:

./mi_practica:
archivo1.txt  archivo2.txt  carpeta1  carpeta2

./mi_practica/carpeta1:

./mi_practica/carpeta2:

./música:

./proyecto:
src

./proyecto/src:
main

./proyecto/src/main:

./proyecto_final:
codigo  documentacion  recursos

./proyecto_final/codigo:
config.json  main.py

./proyecto_final/documentacion:
README.md

./proyecto_final/recursos:

./trabajo:
informe.txt  notas.md

./videos:

- Pregunta de reflexion: ¿Cómo ayuda la opción R a explorar directorios grandes?
- Proporciona una visión jerárquica completa del proyecto sin necesidad de entrar manualmente en cada carpeta. Es ideal para verificar estructuras de software, localizar archivos perdidos en subniveles o auditar la organización de un repositorio de un solo vistazo. Pero debemos saber tambien, que al ser jerarquicamente, nos llenara la terminal y la podremos saturar, asi que debemos saber cuando utilizarla. 

# Laboratorio 7: Combinando Opciones (lah):
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lah
total 11M
drwxrwxrwx+ 14 codespace root      4.0K Feb 22 18:48 .
drwxr-xrwx+  5 codespace root      4.0K Feb 21 23:26 ..
drwxrwxrwx+  8 codespace root      4.0K Feb 22 00:51 .git
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:33 .mi_archivo_secreto
-rw-rw-rw-   1 codespace root       23K Feb 22 18:53 README.md
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo3.txt
-rw-rw-rw-   1 codespace codespace  10M Feb 22 18:42 archivo_grande
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:48 biblioteca
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:42 documentos
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 fotos
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:50 mi_Proyecto
drwxrwxrwx+  3 codespace codespace 4.0K Feb 22 18:48 mi_directorio
drwxrwxrwx+  4 codespace codespace 4.0K Feb 22 18:25 mi_practica
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 música
drwxrwxrwx+  3 codespace codespace 4.0K Feb 21 23:46 proyecto
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:27 proyecto_final
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:46 prueba.txt
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:47 trabajo
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 videos

- Despues de crear la carpeta o directorio secretos, y 3 archivos dentro de este quedaria asi:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir secretos
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd secretos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/secretos (main) $ touch fotos documentos sistema

@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lah
total 11M
drwxrwxrwx+ 15 codespace root      4.0K Feb 22 18:54 .
drwxr-xrwx+  5 codespace root      4.0K Feb 21 23:26 ..
drwxrwxrwx+  8 codespace root      4.0K Feb 22 00:51 .git
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:33 .mi_archivo_secreto
-rw-rw-rw-   1 codespace root       25K Feb 22 18:56 README.md
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 21 23:40 archivo3.txt
-rw-rw-rw-   1 codespace codespace  10M Feb 22 18:42 archivo_grande
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:48 biblioteca
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:42 documentos
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 fotos
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:50 mi_Proyecto
drwxrwxrwx+  3 codespace codespace 4.0K Feb 22 18:48 mi_directorio
drwxrwxrwx+  4 codespace codespace 4.0K Feb 22 18:25 mi_practica
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 música
drwxrwxrwx+  3 codespace codespace 4.0K Feb 21 23:46 proyecto
drwxrwxrwx+  5 codespace codespace 4.0K Feb 21 23:27 proyecto_final
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:46 prueba.txt
drwxrwxrwx+  2 codespace codespace 4.0K Feb 22 18:54 secretos
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:47 trabajo
drwxrwxrwx+  2 codespace codespace 4.0K Feb 21 23:44 videos

Como vemos, estoy puesto en practica terminal, y con el comando (ls -lah) podemos ver quiénes están en la carpeta actual, pero no el contenido de los subdirectorios.

# Laboratorio 8: Filtrando Archivos por Tipo:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -d */
biblioteca/  documentos/  fotos/  mi_Proyecto/  mi_directorio/  mi_practica/  música/  proyecto/  proyecto_final/  secretos/  trabajo/  videos/

- Luego de crear una carpeta codigo, al volver a listar nuevamente con el mismo comando, veamos la salida de la terminal:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -d */
biblioteca/  codigo/  documentos/  fotos/  mi_Proyecto/  mi_directorio/  mi_practica/  música/  proyecto/  proyecto_final/  secretos/  trabajo/  videos/

# Laboratorio 9: Mostrando Permisos y Propietarios
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
total 10320
-rw-rw-rw-  1 codespace root         27446 Feb 22 19:06 README.md
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace        0 Feb 21 23:40 archivo3.txt
-rw-rw-rw-  1 codespace codespace 10485760 Feb 22 18:42 archivo_grande
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace     4096 Feb 22 19:05 codigo
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:42 documentos
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 fotos
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 3 codespace codespace     4096 Feb 22 18:48 mi_directorio
drwxrwxrwx+ 4 codespace codespace     4096 Feb 22 18:25 mi_practica
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 música
drwxrwxrwx+ 3 codespace codespace     4096 Feb 21 23:46 proyecto
drwxrwxrwx+ 5 codespace codespace     4096 Feb 21 23:27 proyecto_final
-rw-rw-rw-  1 codespace codespace        0 Feb 22 18:46 prueba.txt
drwxrwxrwx+ 2 codespace codespace     4096 Feb 22 18:54 secretos
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:47 trabajo
drwxrwxrwx+ 2 codespace codespace     4096 Feb 21 23:44 videos

 Ejercicio practico: Comando utilizado: chmod a-w archivo1.txt: 
- Resultado: Se eliminaron los permisos de escritura para todos los usuarios (all - write).
- Observación: Al ejecutar ls -l, este nos confirma que las letras w desaparecieron del archivo al listarlo. Esto protege nuestro archivo contra modificaciones accidentales. Si intentamos guardar cambios dentro de el en este momento, el sistema nos lanzara un error de "Permiso denegado".

# Laboratorio 10: Desafío Final:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p Proyecto/{documentos,imagenes,temp}

touch Proyecto/documentos/reporte.txt

touch Proyecto/imagenes/foto.jpg

touch Proyecto/temp/archivo_temporal

- Con comando ls -a: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git                 Proyecto   archivo1.txt  archivo3.txt    biblioteca  documentos  mi_Proyecto    mi_practica  proyecto        prueba.txt  trabajo
..  .mi_archivo_secreto  README.md  archivo2.txt  archivo_grande  codigo      fotos       mi_directorio  música       proyecto_final  secretos    videos

- Con comando ls -lh: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lh
total 11M
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 22 19:11 Proyecto
-rw-rw-rw-  1 codespace root       30K Feb 22 19:13 README.md
-r--r--r--  1 codespace codespace    0 Feb 21 23:40 archivo1.txt
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo2.txt
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:40 archivo3.txt
-rw-rw-rw-  1 codespace codespace  10M Feb 22 18:42 archivo_grande
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 21 23:48 biblioteca
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 22 19:05 codigo
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:42 documentos
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:44 fotos
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 21 23:50 mi_Proyecto
drwxrwxrwx+ 3 codespace codespace 4.0K Feb 22 18:48 mi_directorio
drwxrwxrwx+ 4 codespace codespace 4.0K Feb 22 18:25 mi_practica
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:44 música
drwxrwxrwx+ 3 codespace codespace 4.0K Feb 21 23:46 proyecto
drwxrwxrwx+ 5 codespace codespace 4.0K Feb 21 23:27 proyecto_final
-rw-rw-rw-  1 codespace codespace    0 Feb 22 18:46 prueba.txt
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 22 18:54 secretos
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:47 trabajo
drwxrwxrwx+ 2 codespace codespace 4.0K Feb 21 23:44 videos

- Con el comando ls -d */: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -d */
Proyecto/    codigo/      fotos/        mi_directorio/  música/    proyecto_final/  trabajo/
biblioteca/  documentos/  mi_Proyecto/  mi_practica/    proyecto/  secretos/        videos/

- Podemos ver que la diferente manera de listarlos nos saca diferentes resultados en la terminal, por el comando que coloquemos despues del principal que seria (ls)

# Pregunta de Reflexión: ¿Qué opción usarías para encontrar rápidamente un archivo oculto importante?
Respuesta:
- Usaría ls -a. Es la única forma de que la terminal te muestre los archivos que empiezan con un punto (.), ya que el sistema los oculta por defecto para no llenar la vista de archivos de configuración.
