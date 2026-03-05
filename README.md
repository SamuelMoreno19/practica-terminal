# practica-terminal
# Ejercicio practico - leccion #1
Crea un directorio llamado proyecto_final: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir proyecto_final
Entramos a nuestro directorio creado: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd  proyecto_final
Dentro de proyecto_final, creamos los 3 subdirectorios (codigo, documentacion y recursos): @SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ mkdir codigo documentacion recursos
Dentro del directorio codigo, creamos los archivos(main.py, config.json): @SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ touch codigo/main.py codigo/config.json
Dentro del directorio documentacion, crea un archivo llamado README.md: @SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ touch documentacion/README.md
En este comando tree no estaba descargado asi que nos salio error: @SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ tree proyecto_final
proyecto_final  [error opening dir]

0 directories, 0 files

Nos devolvemos al directori@o principal para colocar tree nuevamente: SamuelMoreno19 ➜ /workspaces/practica-terminal/proyecto_final (main) $ cd ..
Verifica la estructura con tree: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree proyecto_final
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
Usa el comando touch para crear un archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba.txt
Verifica que el archivo se haya creado usando el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  proyecto_final  prueba.txt

# Laboratorio 2: Crear múltiples archivos:
El comando touch se utiliza para crear archivos vacíos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo1.txt archivo2.txt archivo3.txt
Verifica que el archivo se haya creado usando el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  archivo1.txt  archivo2.txt  archivo3.txt  proyecto_final  prueba.txt

# Laboratorio 3: Actualizar la marca de tiempo de un archivo:
Se crea un archivo con el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) touch prueba.txt
muestra información detallada del archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
-rw-rw-rw-  1 codespace codespace    0 Feb 21 23:41 prueba.txt

# Laboratorio 4: Crear un directorio simple
crea una carpeta llamada documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir documentos
Verifica que el archivo se haya creado usando el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  archivo1.txt  archivo2.txt  archivo3.txt  documentos  proyecto_final  prueba.txt

# Laboratorio 5: Crear múltiples directorios
permite crear varias carpetas al mismo tiempo con mdkir: SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir fotos videos música
Verifica que el archivo se haya creado usando el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md documentos fotos  música  proyecto_final videos

# Laboratorio 6: Crear directorios anidados
permite crear varios directorios dentro de otros en un solo comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p proyecto/src/main
muestra la estructura de carpetas creada. @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree proyecto
proyecto
└── src
    └── main
3 directories, 0 files

# Laboratorio 7: Combinar archivos y directorios
Se crea la carpeta trabajo y dentro de ella dos archivos: SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir trabajo
touch trabajo/informe.txt trabajo/notas.md
muestra los archivos que contiene la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls trabajo
informe.txt  notas.md

# Laboratorio 8: Crear una estructura compleja:
Se crean varias carpetas dentro de biblioteca usando {}. Luego se agregan archivos en algunas de ellas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p biblioteca/{libros,revistas,artículos}
touch biblioteca/libros/novela.txt biblioteca/revistas/ciencia.md
muestra toda la estructura: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree biblioteca
biblioteca
├── artículos
├── libros
│   └── novela.txt
└── revistas
    └── ciencia.md
4 directories, 2 files

# Laboratorio 9: Proyecto final: 
Se crea una carpeta con el respectivo comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir mi_Proyecto
Se ingresa a la carpeta creada brevemente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd  mi_Proyecto
Creamos 3 subcarpetas dentro de la carpeta principal: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ mkdir codigo documentacion recursos
Creamos los archivos dentro de las subcarpetas: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ touch codigo/main.py codigo/config.json
Creamos un archivo readme: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ touch documentacion/README.md
permite subir un nivel en el directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_Proyecto (main) $ cd ..
Observamos la estructura de la carpeta y sus subcarpetas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ tree mi_Proyecto
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
cd cambia al directorio /var/log: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd /var/log
muestra la ruta actual.: @SamuelMoreno19 ➜ /var/log $ pwd
/var/log

permite subir un nivel en el directorio: @SamuelMoreno19 ➜ /var/log $ cd ..
muestra que ahora estamos en /var.: @SamuelMoreno19 ➜ /var $ pwd
/var

cd - regresa al directorio anterior: @SamuelMoreno19 ➜ /var $ cd -
/var/log
onfirma que volvimos a /var/log.: @SamuelMoreno19 ➜ /var/log $ pwd
/var/log

lleva al directorio personal del usuario: @SamuelMoreno19 ➜ /var/log $ cd ~
muestra la ruta del home (/home/codespace): @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace

# Laboratorio 1: Comprender el Directorio Actual:
muestra la ruta del directorio actual en el que estamos trabajando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ pwd
/workspaces/practica-terminal.
La ruta /workspaces/practica-terminal se divide de la siguiente manera:
- /(Raíz): Es el directorio raíz del sistema de archivos de Linux. Todo comienza aquí.
- workspaces/: Es una carpeta de primer nivel dentro de la raíz, utilizada comúnmente en entornos como GitHub Codespaces para agrupar los proyectos.
- practica-terminal/: Es el nombre de tu repositorio o carpeta específica de trabajo. Es donde estás creando todos tus archivos y laboratorios.
- El pwd lo que nos ayuda es a que no nos sintamos perdidos en nuestros directorios y saber en donde estamos dentro de nuestra maquina 

# Laboratorio 2: Cambiar al Directorio Raíz:
nos lleva al directorio raíz del sistema Linux: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd /
pwd confirma que estamos en /: @SamuelMoreno19 ➜ / $ pwd
/
ls muestra los directorios principales del sistema, como bin, home, usr, var, entre otros: @SamuelMoreno19 ➜ / $ ls
bin                boot  etc  home  lib.usr-is-merged  lib64  mnt  proc  run   sbin.usr-is-merged  sys  usr  vscode
bin.usr-is-merged  dev   go   lib   lib32              media  opt  root  sbin  srv                 tmp  var  workspaces
- Y como podemos observar con el comando (ls) nos suelta 13 directorios principales al menos en mi maquina de trabajo.

# Laboratorio 3: Navegar a un Directorio Específico:
nos lleva al directorio home del sistema: @SamuelMoreno19 ➜ / $ cd /home
muestra la ruta actual (/home): @SamuelMoreno19 ➜ /home $ pwd
/home
lista las carpetas dentro de ese directorio: @SamuelMoreno19 ➜ /home $ ls
codespace  vscode
Luego cd codespace entra a esa carpeta específica: @SamuelMoreno19 ➜ /home $ cd codespace
pwd confirma que ahora estamos en /home/codespace: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace

# Laboratorio 4: Uso de Rutas Relativas:
muestra el directorio actual: @SamuelMoreno19 ➜ / $ pwd
/
nos lleva al directorio del usuario: @SamuelMoreno19 ➜ / $ cd /home/codespace
muestra el directorio actual: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
Luego cd ../../workspaces/practica-terminal/documentos usa rutas relativas (.. para subir niveles) hasta llegar a la carpeta documentos: @SamuelMoreno19 ➜ ~ $ cd ../../workspaces/practica-terminal/documentos
confirma la nueva ruta: @SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ pwd
/workspaces/practica-terminal/documentos

# Laboratorio 5: Volver al Directorio Anterior:
cambia al directorio /tmp: SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd /tmp
muestra la ruta actual: @SamuelMoreno19 ➜ /tmp $ pwd
/tmp
permite volver al directorio anterior: @SamuelMoreno19 ➜ /tmp $ cd -
/workspaces/practica-terminal/documentos
Si lo ejecutamos varias veces este alterna entre los 2 ultimos directorios que visitamos: @SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd -
/tmp
@SamuelMoreno19 ➜ /tmp $ cd -
/workspaces/practica-terminal/documentos
@SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd - 
/tmp

# Laboratorio 6: Ir al Directorio Personal:
lleva al directorio personal del usuario: @SamuelMoreno19 ➜ /tmp $ cd ~
confirma la ruta: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
crea un archivo vacío. @SamuelMoreno19 ➜ ~ $ touch prueba.txt
confirma la ruta: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
muestra los archivos y carpetas dentro del directorio personal: @SamuelMoreno19 ➜ ~ $ ls
java  nvm  prueba.txt

# Laboratorio 7: Subir un Nivel en el Sistema de Archivos:
muestra el directorio actual: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
cd ../.. usa rutas relativas para subir dos niveles en la estructura de carpetas hasta llegar al directorio raíz /:@SamuelMoreno19 ➜ ~ $ cd ../..
confirma la nueva ubicación: @SamuelMoreno19 ➜ / $ pwd
/

# Laboratorio 8: Combinar Rutas Relativas y Absolutas:
usa una ruta absoluta para ir directamente a /home: @SamuelMoreno19 ➜ / $ cd /home
muestra el directorio actual: @SamuelMoreno19 ➜ /home $ pwd
/home
cd codespace usa una ruta relativa para entrar a esa carpeta desde /home: @SamuelMoreno19 ➜ /home $ cd codespace
muestra el directorio actual: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
Luego cd /home vuelve a usar una ruta absoluta para regresar a ese directorio: @SamuelMoreno19 ➜ ~ $ cd /home
muestra el directorio actual: @SamuelMoreno19 ➜ /home $ pwd
/home
La gran diferencia:
- Ruta Absoluta: Es como la dirección de una casa con calle, carrera y número (ej. /home/codespace). Empieza siempre desde la raíz (/) y funciona sin importar dónde estés.
- Ruta Relativa: Es como decir "pasa a la habitación de al lado". Depende de dónde estés parado y no empieza con /.

# Laboratorio 9: Crear y Navegar a un Nuevo Directorio: 
crea una carpeta llamada pruebas en el directorio personal: @SamuelMoreno19 ➜ /home $ mkdir ~/pruebas
entra a esa carpeta: @SamuelMoreno19 ➜ /home $ cd  ~/pruebas
crea otra carpeta dentro de pruebas: @SamuelMoreno19 ➜ ~/pruebas $ mkdir nivell
permite acceder a ella: @SamuelMoreno19 ➜ ~/pruebas $ cd nivell
muestra el directorio actual: @SamuelMoreno19 ➜ ~/pruebas/nivell $ pwd
/home/codespace/pruebas/nivell
lista el contenido del directorio (en este caso está vacío): @SamuelMoreno19 ➜ ~/pruebas/nivell $ ls
@SamuelMoreno19 ➜ ~/pruebas/nivell $

# Laboratorio 10: Explorar Directorios Ocultos:
muestra el directorio actual: @SamuelMoreno19 ➜ ~ $ pwd
/home/codespace
ista todos los archivos, incluyendo los ocultos (los que empiezan con .): @SamuelMoreno19 ➜ ~ $ ls -a
.              .bash_logout  .conda   .dotnet     .jupyter  .minikube   .php      .rbenv  .vscode-remote  java        pruebas
..             .bashrc       .config  .gitconfig  .local    .nvs        .profile  .ruby   .zprofile       nvm
.bash_history  .cache        .docker  .hugo       .maven    .oh-my-zsh  .python   .rvmrc  .zshrc          prueba.txt
permite entrar a un directorio oculto: @SamuelMoreno19 ➜ ~ $ cd .config
confirma la nueva ruta: @SamuelMoreno19 ➜ ~/.config $ pwd
/home/codespace/.config
Los directorios que comienzan con un punto (.) están ocultos por dos razones:
- Orden visual: Evitan llenar la carpeta personal de archivos que el usuario no usa diariamente.
- Seguridad: Protegen archivos de configuración críticos contra modificaciones accidentales que podrían afectar el funcionamiento del sistema o las aplicaciones.

# Leccion 3 # Listando Contenidos con ls y sus Opciones en Linux:
# Sección 4: Ejercicios Prácticos:
# Ejercicio 1: Explora tu directorio actual:
muestra todos los archivos y carpetas visibles que existen en el directorio actual: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md  archivo1.txt  archivo2.txt  archivo3.txt  biblioteca  documentos  fotos  mi_Proyecto  música  proyecto  proyecto_final  prueba.txt  trabajo  videos

# Ejercicio 2: Encuentra archivos ocultos:
muestra todos los archivos, incluyendo los ocultos (los que empiezan con .), como .git: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git       archivo1.txt  archivo3.txt  documentos  mi_Proyecto  proyecto        prueba.txt  videos
..  README.md  archivo2.txt  biblioteca    fotos       música       proyecto_final  trabajo

# Ejercicio 3: Analiza los permisos:
muestra una lista detallada de los archivos y directorios, incluyendo permisos, propietario, tamaño y fecha de modificación: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
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
ls -l muestra la información detallada de los archivos,
-a incluye los archivos ocultos,
y -h muestra los tamaños en un formato más fácil de leer (KB, MB, etc.): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lah
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
Se crea la carpeta mi_practica: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir mi_practica
se entra en ella: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd  mi_practica
Luego se crean dos archivos: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ touch archivo1.txt archivo2.txt 
Luego creamos 2 carpetas o directorios: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ mkdir carpeta1 carpeta2
ls -l muestra la información detallada de los archivos,
-a incluye los archivos ocultos,
y -h muestra los tamaños en un formato más fácil de leer (KB, MB, etc.): @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ ls -lah
total 16K
drwxrwxrwx+  4 codespace codespace 4.0K Feb 22 18:25 .
drwxrwxrwx+ 13 codespace root      4.0K Feb 22 18:24 ..
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:25 archivo1.txt
-rw-rw-rw-   1 codespace codespace    0 Feb 22 18:25 archivo2.txt
drwxrwxrwx+  2 codespace codespace 4.0K Feb 22 18:25 carpeta1
drwxrwxrwx+  2 codespace codespace 4.0K Feb 22 18:25 carpeta2
muestra la estructura completa de carpetas y archivos de forma recursiva: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ ls -R
.:
archivo1.txt  archivo2.txt  carpeta1  carpeta2
./carpeta1:
./carpeta2:

# Laboratorio 1: Exploración Básica del Directorio Actual:
muestra los archivos y carpetas dentro de mi_practica: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ ls
archivo1.txt  archivo2.txt  carpeta1  carpeta2
permite entrar a esa carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica (main) $ cd carpeta1
Al ejecutar ls nuevamente, no aparece nada porque la carpeta está vacía: @SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica/carpeta1 (main) $ ls
@SamuelMoreno19 ➜ /workspaces/practica-terminal/mi_practica/carpeta1 (main)
- Aqui podemos ver que al ejecutar el comando (ls) aparecen 2 archivos .txt, y 2 directorios los cuales son carpeta 1 y 2
- Pregunta de Reflexión: ¿Qué sucede si ejecutas ls en un directorio vacío?
- Si yo entro a una carpeta que no tiene nada o directorio (como mi carpeta1) y escribo el comando ls, la terminal no me mostrará nada. Simplemente una nueva linea de terminal para seguir colocando nuevos comandos, como el directorio esta vacio

# Laboratorio 2: Descubriendo Archivos Ocultos:
muestra todos los archivos, incluidos los ocultos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git       archivo1.txt  archivo3.txt  documentos  mi_Proyecto  música    proyecto_final  trabajo
..  README.md  archivo2.txt  biblioteca    fotos       mi_practica  proyecto  prueba.txt      videos

crea un archivo oculto (porque empieza con .): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch .mi_archivo_secreto
Al ejecutar ls -a nuevamente se puede ver el archivo oculto: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git                 README.md     archivo2.txt  biblioteca  fotos        mi_practica  proyecto        prueba.txt  videos
..  .mi_archivo_secreto  archivo1.txt  archivo3.txt  documentos  mi_Proyecto  música       proyecto_final  trabajo
Con ls normal no aparece porque los archivos ocultos no se muestran por defecto: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
README.md     archivo2.txt  biblioteca  fotos        mi_practica  proyecto        prueba.txt  videos
archivo1.txt  archivo3.txt  documentos  mi_Proyecto  música       proyecto_final  trabajo
- Respuesta a la Pregunta de Reflexión: ¿Por qué algunos archivos están ocultos por defecto?
- Limpieza Visual: Como ya vimos en mi salida de la terminal, tengo archivos como .git o .mi_archivo_secreto. Si todos los archivos de configuración (que suelen ser muchos) estuvieran visibles, me seria mucho mas dificil encontrar tus carpetas importantes.
- Seguridad (Evitar accidentes): Al estar ocultos, es menos probable que los borres o los cambies por error. Normalmente, los archivos ocultos son la "columna vertebral" de mis programas o de Git; si no los ves, no se pueden cambiar o dañar.

# Laboratorio 3: Entendiendo los Detalles con l:
crea el archivo si no existe o actualiza su fecha de modificación si ya existe: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba.txt
muestra la información detallada del archivo, como permisos, propietario, tamaño y fecha: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
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
uestra la información detallada de los archivos y -h muestra los tamaños en formato legible (KB, MB, etc.): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lh
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

Crea un archivo de 10 MB lleno de ceros: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ dd if=/dev/zero of=archivo_grande bs=1M count=10
10+0 records in
10+0 records out
10485760 bytes (10 MB, 10 MiB) copied, 0.00819897 s, 1.3 GB/s

# Pregunta de Reflexión: ¿Por qué es útil mostrar el tamaño en formato legible?
- Interpretación Rápida: No es lo mismo leer 1073741824 que leer 1G. El formato humano te permite saber al instante si un archivo es pesado o liviano sin tener que contar dígitos o hacer divisiones mentales.

Prevención de Errores: Al ver unidades como K (Kilobytes), M (Megabytes) o G (Gigabytes), puedes identificar rápidamente archivos que estén llenando el disco duro innecesariamente.

# Laboratorio 5: Ordenando por Tiempo de Modificación:
muestra información detallada y -t ordena los archivos por fecha de modificación, mostrando primero los más recientes: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lt
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
muestra información detallada y -t ordena los archivos por fecha de modificación, mostrando primero los más recientes: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lt
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
crea directorios anidados de una vez, crea archivos dentro de diferentes niveles de la estructura de carpetas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p mi_directorio/subdirectorio1/subdirectorio2
touch mi_directorio/archivo1.txt
touch mi_directorio/subdirectorio1/archivo2.txt

muestra todos los archivos y carpetas, incluyendo los contenidos de los subdirectorios, de manera recursiva: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -R
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
ls -l muestra información detallada (permisos, propietario, tamaño, fecha), -a incluye archivos ocultos, y -h muestra los tamaños en formato legible (KB, MB, etc.): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lah
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
Se crea la carpeta secretos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir secretos
Nos dirigimos dentro de la carpeta secretos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd secretos
dentro de ella tres archivos vacíos (fotos, documentos, sistema) usando touch: @SamuelMoreno19 ➜ /workspaces/practica-terminal/secretos (main) $ touch fotos documentos sistema

ls -l muestra información detallada (permisos, propietario, tamaño, fecha),
-a incluye archivos ocultos,
y -h muestra los tamaños en formato legible (KB, MB, etc.): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lah
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
muestra solo los directorios del directorio actual, filtrando los archivos normales: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -d */
biblioteca/  documentos/  fotos/  mi_Proyecto/  mi_directorio/  mi_practica/  música/  proyecto/  proyecto_final/  secretos/  trabajo/  videos/

- Luego de crear una carpeta codigo, al volver a listar nuevamente con el mismo comando, veamos la salida de la terminal:
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -d */
biblioteca/  codigo/  documentos/  fotos/  mi_Proyecto/  mi_directorio/  mi_practica/  música/  proyecto/  proyecto_final/  secretos/  trabajo/  videos/

# Laboratorio 9: Mostrando Permisos y Propietarios
muestra detalles completos de cada archivo y carpeta, incluyendo permisos, propietario, tamaño y fecha de modificación: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l
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
Se crea una estructura de carpetas (Proyecto) dentro de Proyecto se crean subdirectorios y se agregan archivos específicos en cada subcarpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p Proyecto/{documentos,imagenes,temp}

touch Proyecto/documentos/reporte.txt

touch Proyecto/imagenes/foto.jpg

touch Proyecto/temp/archivo_temporal

- Con comando ls -a, muestra todos los archivos y carpetas, incluidos los ocultos (los que comienzan con .): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -a
.   .git                 Proyecto   archivo1.txt  archivo3.txt    biblioteca  documentos  mi_Proyecto    mi_practica  proyecto        prueba.txt  trabajo
..  .mi_archivo_secreto  README.md  archivo2.txt  archivo_grande  codigo      fotos       mi_directorio  música       proyecto_final  secretos    videos

- Con comando ls -lh, muestra información detallada (permisos, propietario, fecha, etc.) y -h muestra los tamaños en formato legible (KB, MB, etc.): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -lh
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

- Con el comando ls -d */, ista únicamente los directorios dentro del directorio actual, sin mostrar archivos normales: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -d */
Proyecto/    codigo/      fotos/        mi_directorio/  música/    proyecto_final/  trabajo/
biblioteca/  documentos/  mi_Proyecto/  mi_practica/    proyecto/  secretos/        videos/

- Podemos ver que la diferente manera de listarlos nos saca diferentes resultados en la terminal, por el comando que coloquemos despues del principal que seria (ls)

# Pregunta de Reflexión: ¿Qué opción usarías para encontrar rápidamente un archivo oculto importante?
Respuesta:
- Usaría ls -a. Es la única forma de que la terminal te muestre los archivos que empiezan con un punto (.), ya que el sistema los oculta por defecto para no llenar la vista de archivos de configuración.

# Leccion 4 copiar archivos y directorios con el comando cp en Linux
- Ejercicio 1: Copiar un archivo:
crea el archivo @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba2.txt
cp copia el archivo a copia_prueba2.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp prueba2.txt copia_prueba2.txt
ls muestra ambos archivos en el directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto   archivo1.txt  archivo3.txt biblioteca  copia_prueba2.txt fotos mi_directorio  música proyecto_final prueba2.txt  trabajo
README.md  archivo2.txt  archivo_grande  codigo documentos  mi_Proyecto  mi_practica proyecto  prueba.txt      secretos     videos

- Ejercicio 2: Copiar un directorio:
mkdir crea la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir carpeta1
Creamos un archivo dentro de la carpeta creada anteriormente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch carpeta1/archivo1.txt
cp -r copia recursivamente todo el contenido de carpeta1 a carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -r carpeta1 carpeta2
ls carpeta2 confirma que la copia contiene archivo1.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls carpeta2
archivo1.txt

- Ejercicio 3: Usar opciones avanzadas:
-f fuerza la sobrescritura si el archivo ya existe en el destino.
-v muestra en pantalla qué archivos se están copiando.
La salida confirma que archivo1.txt fue copiado a carpeta2: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -fv carpeta1/archivo1.txt carpeta2/
'carpeta1/archivo1.txt' -> 'carpeta2/archivo1.txt'

# Laboratorio 1: Copiar un archivo simple:
Crea un archivo vacío llamado archivo.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo.txt
Toma el archivo original (origen) y crea un duplicado exacto con el nuevo nombre (destino): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo1.txt copia_archivo1.txt
Toma el archivo original (origen) y crea un duplicado exacto con el nuevo nombre (destino): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo.txt copia_archivo.txt
Lo usamos para verificar que ahora existen ambos archivos en la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto     archivo1.txt  archivo_grande  carpeta2           copia_prueba2.txt  mi_Proyecto    música          prueba.txt   trabajo
README.md    archivo2.txt  biblioteca      codigo             documentos         mi_directorio  proyecto        prueba2.txt  videos
archivo.txt  archivo3.txt  carpeta1        copia_archivo.txt  fotos              mi_practica    proyecto_final  secretos

- Preguntas de reflexion : Preguntas de Reflexión:
- ¿Qué sucede si el archivo origen no existe: La terminal arroja un error (No such file or directory) y no realiza ninguna copia.
- ¿Qué pasa si el archivo de destino ya existe: El comando cp lo sobrescribe automáticamente sin pedir confirmación, reemplazando el contenido viejo por el nuevo.

# Laboratorio 2: Copiar un archivo a otro directorio:
Creamos la carpeta llamada documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir documentos
copia el archivo dentro de esa carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo1.txt documentos/
cd documentos entra al directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cd documentos
ls confirma que el archivo fue copiado correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ ls
archivo1.txt

- Preguntas de reflexion: ¿Qué sucede si el directorio de destino no existe: el comando cp no creara la carpeta automáticamente sino que en su lugar, tratará el destino como un nombre de archivo nuevo y copiará el origen ahí.
- ¿Cómo puedes copiar un archivo a un directorio fuera del directorio actual: Aca debemos utilizar las rutas, como los siguientes ejemplos: 
Ruta relativa: cp archivo.txt ../otra_carpeta/ (sube un nivel).
Ruta absoluta: cp archivo.txt /home/usuario/documentos/ (ruta completa).

# Laboratorio 3: Copiar múltiples archivos:
Sube al directorio padre desde documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal/documentos (main) $ cd ..
crea tres archivos nuevos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo2.txt archivo3.txt archivo4.txt
los copia todos a la carpeta documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo2.txt archivo3.txt archivo4.txt documentos/
ls documentos/ confirma que ahora contiene todos los archivos (archivo1.txt a archivo4.txt): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos/
archivo1.txt  archivo2.txt  archivo3.txt  archivo4.txt

- Preguntas de reflexion: ¿Qué sucede si uno de los archivos no existe: nuestro comando (cp) copiará todos los archivos que si pueda encontrar, pero lanzará un mensaje de error por cada archivo que no exista. La operación no se detiene y sigue trabajando.
- Cómo puedes copiar todos los archivos .txt de un directorio: Usando el comodín asterisco (wildcard): cp *.txt destino/. Esto selecciona automáticamente cualquier archivo que termine con esa extensión.

# Laboratorio 4: Copiar un directorio completo:
Se crea la carpeta proyectos con dos archivos dentro: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir proyectos
touch proyectos/archivo5.txt proyectos/archivo6.txt
cp -r copia recursivamente todo el directorio y su contenido a proyectos_copia: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -r proyectos proyectos_copia
ls proyectos_copia/ confirma que los archivos se copiaron correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls proyectos_copia/
archivo5.txt  archivo6.txt

- Preguntas de reflexion: ¿Qué sucede si omites la opción r al copiar un directorio: El comando fallará y mostrará un error (omitting directory). cp no puede copiar carpetas por defecto si no se le indica que sea recursivo.
- ¿Cómo copiar solo ciertos archivos dentro de un directorio: Usando patrones o comodines. Por ejemplo:
- cp proyectos/*.jpg destino/ (solo imágenes JPG).
- cp proyectos/archivo[1-3].txt destino/ (solo los archivos del 1 al 3).

# Laboratorio 5: Forzar la sobrescritura de archivos:
touch crea archivo7.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo7.txt
cp lo copia a la carpeta documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo7.txt documentos/
cp -f fuerza la sobrescritura si ya existiera un archivo con el mismo nombre: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -f archivo7.txt documentos/
ls documentos/ confirma que archivo7.txt está en la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos/
archivo1.txt  archivo2.txt  archivo3.txt  archivo4.txt  archivo7.txt

- Preguntas reflexion: ¿Qué sucede si no usas la opción f: El archivo se sobrescribe directamente y de forma silenciosa. No aparece ningún mensaje de advertencia en la terminal.
- ¿Cómo puedes evitar que se sobrescriba un archivo existente: Omitiendo la opción -f y verificando manualmente con ls antes de copiar, ya que por defecto el comando no pide confirmación.

# Laboratorio 6: Mostrar mensajes detallados:
-v (verbose) muestra en pantalla qué archivos se están copiando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -v archivo7.txt documentos/
'archivo7.txt' -> 'documentos/archivo7.txt
-f fuerza la sobrescritura si el archivo ya existe.
La salida confirma que archivo7.txt fue copiado a documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -fv archivo7.txt documentos/
'archivo7.txt' -> 'documentos/archivo7.txt'

- ¿Qué información adicional muestra la opción v: Muestra la confirmación visual de la operación, indicando la ruta del archivo original y hacia dónde fue copiado con una flecha: 'origen' -> 'destino'.
- ¿Cómo puedes combinar v con otras opciones como f: Se pueden agrupar después de un solo guion. Por ejemplo, cp -fv aplica tanto la fuerza como el mensaje detallado al mismo tiempo, como se ve en la terminal.

# Laboratorio 7: Preservar atributos de archivos:
Creamos un archivo con el comando touch: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo8.txt
touch -d "2022-01-01" cambia la fecha de modificación del archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch -d "2022-01-01" archivo8.txt
cp -p copia el archivo preservando permisos, propietario y fec: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp -p archivo8.txt copia_archivo8.txt
ls -l muestra que ambos archivos tienen la misma fecha y atributos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls -l archivo8.txt copia_archivo8.txt
-rw-rw-rw- 1 codespace codespace 0 Jan  1  2022 archivo8.txt
-rw-rw-rw- 1 codespace codespace 0 Jan  1  2022 copia_archivo8.txt

- Preguntas de reflexion: ¿Qué atributos se preservan con la opción p: Se preservan los metadatos originales: los permisos y de(lectura, escritura, ejecución), el propietario (owner) y las marcas de tiempo (fecha y hora de la modificación).
- ¿Qué sucede si no usas la opción p: El archivo copiado se crea con los permisos por defecto del sistema y lo más importante, se le asigna la fecha y hora del momento actual, perdiendo la información de cuándo se modificó el original.

# Laboratorio 8: Copiar archivos con patrones:
archivo_*.txt es un patrón que coincide con todos los archivos que empiezan con archivo_ y terminan en .txt:@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo_a.txt archivo_b.txt archivo_c.txt
cp copia todos los archivos que coinciden con el patrón a la carpeta documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo_*.txt documentos/
ls documentos/ confirma que los archivos fueron copiados correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos/
archivo1.txt  archivo2.txt  archivo3.txt  archivo4.txt  archivo7.txt  archivo_a.txt  archivo_b.txt  archivo_c.txt

- Preguntas de reflexion: ¿Qué otros patrones puedes usar para seleccionar archivos: El signo de interrogación (?): Reemplaza exactamente un solo carácter (ej: doc?.txt para doc1.txt, docA.txt) - Los corchetes ([]): Para definir rangos o listas (ej: archivo[1-3].txt para copiar solo el 1, 2 y 3).
- ¿Cómo puedes copiar archivos que terminen con un patrón específico: Usando el asterisco al principio del patrón: cp *patron.extensión destino/. Por ejemplo, para copiar todo lo que termine en "final", usarías cp *final.txt documentos/

# Laboratorio 9: Copiar archivos entre diferentes sistemas de archivos:
Este comando intenta copiar un archivo desde un dispositivo externo (/media/usb) al directorio actual (.).
El error No such file or directory indica que el archivo no existe en la ruta especificada: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp /media/usb/archivo_usb.txt .
cp: cannot stat '/media/usb/archivo_usb.txt': No such file or directory

- Preguntas de reflexion: ¿Qué sucede si el dispositivo USB no está montado: La terminal nos mostrará un error de "archivo o directorio no encontrado" (No such file or directory), ya que el sistema no reconoce la ruta /media/usb como un acceso activo a los archivos.
- ¿Cómo puedes verificar las ubicaciones de los dispositivos conectados: Usando el comando ls /media. Como los USB se montan ahí, listar esa carpeta te permite ver qué dispositivos están disponibles para copiar.

# Laboratorio 10: Resolver errores comunes:
cp: cannot stat significa que el archivo de origen no existe: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo_inexistente.txt documentos/
cp: cannot stat 'archivo_inexistente.txt': No such file or directory, cp: cannot create regular file indica que el destino no es un directorio válido. Siempre hay que verificar que el archivo de origen exista y que el directorio de destino sea correcto antes de copiar: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo1.txt directorio_inexistente/
cp: cannot create regular file 'directorio_inexistente/': Not a directory

- Preguntas de reflexion: ¿Qué mensaje de error recibes cuando el archivo de origen no existe: Como podemos ver en la salida de la terminal (No such file or directory) nos dira que ese archivo o directorio no existe, como era el caso, estabamos probando que nos diria la terminal.
- ¿Qué mensaje de error recibes cuando el directorio de destino no existe:  Aca directamente nos dira que no es un directorio y que esta vez, no existe, entonces como no encuentra una carpeta con ese nombre nos dira (Not a directory) como salida de la terminal. 

# Leccion 5 Moviendo y Renombrando Archivos con el Comando mv en Linux
# Ejercicio 1: Renombrar un archivo:
Creamos el archivo@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo10.txt
mv renombra el archivo a nuevo_nombre.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv archivo10.txt nuevo_nombre.txt
ls muestra que el archivo ahora tiene el nuevo nombre: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto      archivo2.txt  archivo8.txt   archivo_grande  codigo              documentos     mi_practica       proyecto_final   prueba2.txt
README.md     archivo3.txt  archivo_a.txt  biblioteca      copia_archivo.txt   fotos          música            proyectos        secretos
archivo.txt   archivo4.txt  archivo_b.txt  carpeta1        copia_archivo8.txt  mi_Proyecto    nuevo_nombre.txt  proyectos_copia  trabajo
archivo1.txt  archivo7.txt  archivo_c.txt  carpeta2        copia_prueba2.txt   mi_directorio  proyecto          prueba.txt       videos

# Ejercicio 2: Renombrar un directorio
Crea un directorio llamado carpeta_vieja: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir carpeta_vieja
Renombra el directorio a carpeta_nueva: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv carpeta_vieja carpeta_nueva
ls muestra que el archivo ahora tiene el nuevo nombre: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto      archivo2.txt  archivo8.txt   archivo_grande  carpeta_nueva       copia_prueba2.txt  mi_directorio     proyecto         prueba.txt   videos
README.md     archivo3.txt  archivo_a.txt  biblioteca      codigo              documentos         mi_practica       proyecto_final   prueba2.txt
archivo.txt   archivo4.txt  archivo_b.txt  carpeta1        copia_archivo.txt   fotos              música            proyectos        secretos
archivo1.txt  archivo7.txt  archivo_c.txt  carpeta2        copia_archivo8.txt  mi_Proyecto        nuevo_nombre.txt  proyectos_copia  trabajo

# Ejercicio 3: Mover un archivo a otro directorio
Crea un directorio llamado documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir documentos2
Crea un archivo llamado informe.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch informe.txt
Verifica que el archivo se haya movido: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos2/
informe.txt

# Ejercicio 4: Mover múltiples archivos
Crea varios archivos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo5.txt archivo6.txt archivo9.txt
Mueve todos los archivos .txt al directorio documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv *.txt documentos2/
Verifica el contenido del directorio documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos2/
archivo.txt   archivo2.txt  archivo4.txt  archivo6.txt  archivo8.txt  archivo_a.txt  archivo_c.txt      copia_archivo8.txt  informe.txt       prueba.txt
archivo1.txt  archivo3.txt  archivo5.txt  archivo7.txt  archivo9.txt  archivo_b.txt  copia_archivo.txt  copia_prueba2.txt   nuevo_nombre.txt  prueba2.txt

# Ejercicio 5: Mover y renombrar al mismo tiempo
Crea un archivo llamado datos.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch datos.txt
Mueve el archivo datos.txt al directorio documentos y renómbralo como backup_datos.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv datos.txt documentos/backup_datos.txt
Verifica el resultado: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos2/
archivo.txt   archivo3.txt  archivo6.txt  archivo9.txt   archivo_c.txt      copia_archivo8.txt  nuevo_nombre.txt
archivo1.txt  archivo4.txt  archivo7.txt  archivo_a.txt  backup_datos.txt   copia_prueba2.txt   prueba.txt
archivo2.txt  archivo5.txt  archivo8.txt  archivo_b.txt  copia_archivo.txt  informe.txt         prueba2.txt

# Ejercicio 6: Usar la opción i
Crea dos archivos con el mismo nombre en diferentes ubicaciones: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo_existente.txt
touch documentos2/archivo_existente.txt
Intenta mover el archivo del directorio actual al directorio documentos con la opción i: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv -i archivo_existente.txt documentos2/
mv: overwrite 'documentos2/archivo_existente.txt'? y

# Ejercicio 7: Usar la opción u
Crea un archivo en el directorio actual y modifícalo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo_viejo.txt
echo "Contenido viejo" > archivo_viejo.txt
Copia el archivo al directorio documentos2: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo_viejo.txt documentos2/
Modifica el archivo original: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ echo "Contenido nuevo" > archivo_viejo.txt
Usa la opción u para mover el archivo solo si es más reciente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv -u archivo_viejo.txt documentos2/
Verifica el contenido del archivo en el directorio documentos2: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cat documentos2/archivo_viejo.txt
Contenido nuevo

# Desafio final
Crear la base del proyecto: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir proyectos2 
touch crea tres archivos dentro de proyectos2: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch proyectos2/tarea1.txt proyectos2/tarea2.txt proyectos2/tarea3.txt
mv mueve y renombra cada archivo al directorio documentos2 con nuevos nombres (proyecto1.txt, proyecto2.txt, proyecto3.txt): @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv proyectos2/tarea1.txt documentos2/proyecto1.txt mv proyectos2/tarea2.txt documentos2/proyecto2.txt mv proyectos2/tarea3.txt documentos2/proyecto3.txt
ls muestra que el archivo ahora tiene el nuevo nombre: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documentos2
archivo.txt   archivo3.txt  archivo6.txt  archivo9.txt   archivo_c.txt          backup_datos.txt    copia_prueba2.txt  proyecto1.txt  prueba.txt
archivo1.txt  archivo4.txt  archivo7.txt  archivo_a.txt  archivo_existente.txt  copia_archivo.txt   informe.txt        proyecto2.txt  prueba2.txt
archivo2.txt  archivo5.txt  archivo8.txt  archivo_b.txt  archivo_viejo.txt      copia_archivo8.txt  nuevo_nombre.txt   proyecto3.txt

# Laboratorio 1: Renombrar Archivos Simples:
touch crea el archivo prueba1.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba1.txt
mv renombra el archivo a archivo_renombrado.txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv prueba1.txt archivo_renombrado.txt
ls confirma que el archivo ahora aparece con el nuevo nombre: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto        archivo_renombrado.txt  carpeta2       documentos   mi_Proyecto    música          proyectos        secretos
README.md       biblioteca              carpeta_nueva  documentos2  mi_directorio  proyecto        proyectos2       trabajo
archivo_grande  carpeta1                codigo         fotos        mi_practica    proyecto_final  proyectos_copia  videos

# Laboratorio 2: Renombrar Directorios:
mkdir temporal crea la carpeta temporal: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir temporal
mv renombra la carpeta a archivos_temporales: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv temporal archivos_temporales
muestra que el directorio ahora aparece con el nuevo nombre: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto        archivo_renombrado.txt  carpeta1       codigo       fotos          mi_practica  proyecto_final  proyectos_copia  videos
README.md       archivos_temporales     carpeta2       documentos   mi_Proyecto    música       proyectos       secretos
archivo_grande  biblioteca              carpeta_nueva  documentos2  mi_directorio  proyecto     proyectos2      trabajo

# Laboratorio 3: Mover Archivos a Otro Directorio:
mkdir documento crea la carpeta de destino: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir documento
touch informe.txt crea el archivo a mover: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch informe.txt
mv informe.txt documento/ mueve el archivo dentro del directorio document: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv informe.txt documento/
ls documento/ confirma que el archivo ahora está dentro de la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documento/
informe.txt

# Laboratorio 4: Mover Múltiples Archivos:
Creamos los diferentes archivos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo1.txt archivo2.txt archivo3.txt
Creamos la carpeta de destino: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir respaldos
*.txt selecciona todos los archivos que terminan en .txt: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv *.txt respaldos/
ls respaldos/ confirma que los archivos ahora están dentro del directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls respaldos/
archivo1.txt  archivo2.txt  archivo3.txt  archivo_renombrado.txt

# Laboratorio 5: Mover y Renombrar al Mismo Tiempo:
Creamos el archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch datos_originales.txt
Creamops una carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir backup
mv datos_originales.txt backup/datos_backup.txt mueve y renombra el archivo al mismo tiempo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv datos_originales.txt backup/datos_backup.txt
ls backup/ confirma que el archivo ahora se llama datos_backup.txt dentro de backup: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls backup/
datos_backup.txt

# Laboratorio 6: Evitar Sobrescritura con i:
Creamos un archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo_existente.txt
Creamos una carpeta llamada documentos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir documento
mv -i activa el modo interactivo, preguntando antes de sobrescribir archivos existentes: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv -i archivo_existente.txt documento/
mv: overwrite 'documento/archivo_existente.txt'? n
ls documento/ muestra que el archivo existente no fue reemplazado: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls documento/
archivo_existente.txt  informe.txt

# Laboratorio 7: Actualizar Solo Archivos Nuevos con u:
Creamos el archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo_viejo.txt
Crear archivo viejo con contenido inicia: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ echo "Contenido viejo" > archivo_viejo.txt
 Creamos la carpeta respaldo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir respaldo
copiar el archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cp archivo_viejo.txt respaldo/
Modificamos el archivo original: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ echo "Contenido nuevo" > archivo_viejo.txt
Mover solo si es más reciente que el destino: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv -u archivo_viejo.txt respaldo/
Verificar contenido actualizado: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ cat respaldo/archivo_viejo.txt
Contenido nuevo

# Laboratorio 8: Mover Archivos a Rutas Absolutas:
Creamos el archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo_absoluto.txt
mv archivo_absoluto.txt /tmp/ mueve el archivo al directorio /tmp usando una ruta absoluta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv archivo_absoluto.txt /tmp/
ls /tmp/ confirma que el archivo ahora está en el directorio temporal del sistema: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls /tmp/
archivo_absoluto.txt  dockerd.log  storage_version.txt         vscode-ipc-5566146e-c746-438a-b3ec-2f6b25c6ac20.sock
codespaces_logs       sshd.log     vscode-git-d78a5843f5.sock  vscode-ipc-efda31ab-f80a-45b0-b8a8-417ffeb23536.sock

# Laboratorio 9: Mover Archivos con Espacios en el Nombre:
Creamos un archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch "mi archivo.txt"
Creamos una carpeta llamada destino: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir destino
mv "mi archivo.txt" destino/ mueve el archivo preservando el nombre con espacios: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mv "mi archivo.txt" destino/
ls destino/ confirma que el archivo ahora está dentro de destino: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls destino/
'mi archivo.txt'

# Lección 6: Eliminar archivos y directorios con rm y rmdir
# Ejercicio 1: Eliminar archivos específicos:
Creamos un archivo @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch prueba.txt
Y lo eliminamos utilizando el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm prueba.txt

# Ejercicio 2: Eliminar un directorio vacío:
Creamos una carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir temporal
Eliminamos esta carpeta con el comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rmdir temporal

# Ejercicio 3: Eliminar un directorio no vacío:
Creamos una carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir proyecto3
Dentro de esta carpeta creamos los diferentes archivos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch proyecto3/archivo1 proyecto3/archivo2
Aqui eliminamos la carpeta y el contenido dentro de esta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -r proyecto3

# Desafío final:
Creamos tanto carpeta principal como subcarpetas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p proyecto4/{src,docs,tests}
Dentro de esta carpeta, elegimos subcarpetas y creamos sus respectivos archivos: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch proyecto4/src/main.c proyecto4/docs/manual.txt proyecto4/tests/test1.py
Eliminamos absolutamente todo con el siguiente comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -r proyecto4

# Laboratorio 1: Crear y eliminar un archivo básico:
Creamos un archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivo1.txt
Listamos los archivos y carpetas del directorio donde estamos parados: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls 
Proyecto      archivo_existente.txt  backup      carpeta2       destino     documentos2  mi_directorio  proyecto        proyectos2       respaldos  videos
README.md     archivo_grande         biblioteca  carpeta_nueva  documento   fotos        mi_practica    proyecto_final  proyectos_copia  secretos
archivo1.txt  archivos_temporales    carpeta1    codigo         documentos  mi_Proyecto  música         proyectos       respaldo         trabajo
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ 
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm archivo1.txt
@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos          mi_practica  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   mi_Proyecto    música       proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_directorio  proyecto     proyectos2      respaldos        videos

# Laboratorio 2: Eliminar múltiples archivos:
Aqui creamos 3 archivos diferentes: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch archivoA.txt archivoB.txt archivoC.txt
Listamos los archivos y carpetas del directorio donde estamos parados: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto      archivoC.txt           backup      carpeta_nueva  documentos   mi_directorio  proyecto_final   respaldo   videos
README.md     archivo_existente.txt  biblioteca  codigo         documentos2  mi_practica    proyectos        respaldos
archivoA.txt  archivo_grande         carpeta1    destino        fotos        música         proyectos2       secretos
archivoB.txt  archivos_temporales    carpeta2    documento      mi_Proyecto  proyecto       proyectos_copia  trabajo
Aqui eliminamos los archivos creados antes: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm archivoA.txt archivoB.txt archivoC.txt
Volvemos a listar para mirar si se eliminaron: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos          mi_practica  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   mi_Proyecto    música       proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_directorio  proyecto     proyectos2      respaldos        videos

# Laboratorio 3: Eliminar con confirmación:
Creamos un archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch importante.txt
rm -i activa el modo interactivo, preguntando antes de eliminar el archivo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -i importante.txt
Al responder n (no), no se borra el archivo: rm: remove regular empty file 'importante.txt'? n
Al responder y (yes), el archivo importante.txt se elimina del directorio actual: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -i importante.txt
rm: remove regular empty file 'importante.txt'? y

# Laboratorio 4: Eliminar un directorio vacío:
Creamos la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir vacío
Listamos nuevamente todas las carpetas y archivos creados: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivos_temporales  carpeta2       documento    mi_Proyecto    proyecto        proyectos_copia  trabajo
README.md              backup               carpeta_nueva  documentos   mi_directorio  proyecto_final  respaldo         vacío
archivo_existente.txt  biblioteca           codigo         documentos2  mi_practica    proyectos       respaldos        videos
archivo_grande         carpeta1             destino        fotos        música         proyectos2      secretos
Eliminamos solamente el directorio vacio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rmdir vacío
Confirmamos que se elimino al volver a listar todo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos          mi_practica  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   mi_Proyecto    música       proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_directorio  proyecto     proyectos2      respaldos        videos

# Laboratorio 5: Intentar eliminar un directorio no vacío:
Creamos un directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir lleno
Añadimos archivos a esta carpeta creada: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch lleno/archivo1.txt lleno/archivo2.txt
Este comando solo funciona con directorios vacios, y podemos ver el mensaje de error: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rmdir lleno
rmdir: failed to remove 'lleno': Directory not empty

# Laboratorio 6: Eliminar un directorio no vacío con rm -r:
Creamos un directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir proyecto5
Creamos unos archivos dentro de la carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch proyecto5/main.py proyecto/config.json
Listamos lo que creamos anteriormente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivos_temporales  carpeta2       documento    lleno          música          proyectos2       secretos
README.md              backup               carpeta_nueva  documentos   mi_Proyecto    proyecto5       proyectos_copia  trabajo
archivo_existente.txt  biblioteca           codigo         documentos2  mi_directorio  proyecto_final  respaldo         videos
archivo_grande         carpeta1             destino        fotos        mi_practica    proyectos       respaldos
rm -r (recursivo) elimina el directorio proyecto5 junto con todos sus archivos y subdirectorios: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -r proyecto5
ls confirma que el directorio ya no existe en el directorio actual: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos        mi_directorio  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   lleno        mi_practica    proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_Proyecto  música         proyectos2      respaldos        videos

# Laboratorio 7: Eliminar con confirmación recursiva:
Creamos un directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir datos
Creamos 2 archivos dentro de esta carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch datos/registro.txt datos/backup.log
rm -ri datos elimina el directorio y su contenido, pero pregunta por cada archivo y subdirectorio antes de borrarlo y le decimos que (n) y miramos que no lo borra:@SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -ri datos
rm: descend into directory 'datos'? n
Volvemos a colocar el mismo comando pero ahora dandole (y) a la primera pregunta y (n) a las demas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -ri datos
rm: descend into directory 'datos'? y
rm: remove regular empty file 'datos/registro.txt'? n
rm: remove regular empty file 'datos/backup.log'? n
rm: remove directory 'datos'? n
Ahora hacemos nuevamente lo mismo pero colocando (y) en todo y eliminamos todo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -ri datos
rm: descend into directory 'datos'? y
rm: remove regular empty file 'datos/registro.txt'? y
rm: remove regular empty file 'datos/backup.log'? y
rm: remove directory 'datos'? y

# Laboratorio 8: Forzar la eliminación sin confirmación:
Creamos una carpeta: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir temp
touch temp/file1.txt temp/file2.txt crea dos archivos dentro del directorio temp: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch temp/file1.txt temp/file2.txt
ls muestra los archivos y carpetas del directorio actual, confirmando que los archivos se han creado dentro de temp: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivos_temporales  carpeta2       documento    lleno          música          proyectos_copia  temp
README.md              backup               carpeta_nueva  documentos   mi_Proyecto    proyecto_final  respaldo         trabajo
archivo_existente.txt  biblioteca           codigo         documentos2  mi_directorio  proyectos       respaldos        videos
archivo_grande         carpeta1             destino        fotos        mi_practica    proyectos2      secretos

rm -r elimina recursivamente el directorio y todos sus archivos/subdirectorios. -f fuerza la eliminación sin pedir confirmación. En este caso, temp y todos sus archivos (file1.txt, file2.txt) se eliminan de inmediato: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -rf temp
Listamos nuevamente para mirar que si se haya eliminado correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos        mi_directorio  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   lleno        mi_practica    proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_Proyecto  música         proyectos2      respaldos        videos

# Laboratorio 9: Estructura compleja de directorios:
Creamos la carpeta principal y dentro de esta mas subcarpetas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p proyecto3/{src,docs,tests}
Se crea archivos iniciales en cada subdirectorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ touch proyecto3/src/main.c proyecto3/docs/manual.txt proyecto3/tests/test1.py
Listamos todo lo creado anteriormente en nuestro directorio: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivos_temporales  carpeta2       documento    lleno          música          proyectos2       secretos
README.md              backup               carpeta_nueva  documentos   mi_Proyecto    proyecto3       proyectos_copia  trabajo
archivo_existente.txt  biblioteca           codigo         documentos2  mi_directorio  proyecto_final  respaldo         videos
archivo_grande         carpeta1             destino        fotos        mi_practica    proyectos       respaldos
rm -r elimina el directorio proyecto3 y todos sus subdirectorios y archivos de forma recursiva. Esto borra todo lo creado en proyecto3 (src, docs, tests y sus archivos) en un solo comando: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -r proyecto3
Listamos todo nuevamente para mirar que se haya eliminado correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos        mi_directorio  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   lleno        mi_practica    proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_Proyecto  música         proyectos2      respaldos        videos

# Laboratorio 10: Desafío final:
Nuevamente creamos un directorio y subcarpetas dentro de este: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ mkdir -p trabajo/{informes,temporal,archivos} touch trabajo/informes/reporte1.doc trabajo/temporal/notas.txt trabajo/archivos/datos.csv
Listamos para mirar que se haya creado correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos        mi_directorio  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   lleno        mi_practica    proyectos       respaldo         trabajo
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_Proyecto  música         proyectos2      respaldos        videos
rm -r trabajo/temporal elimina el subdirectorio temporal dentro de trabajo: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -r trabajo/temporal
rm -r trabajo elimina todo el directorio trabajo restante con sus archivos y subcarpetas: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ rm -r trabajo
Listamos otra vez para mirar que todo se haya eliminado correctamente: @SamuelMoreno19 ➜ /workspaces/practica-terminal (main) $ ls
Proyecto               archivo_grande       biblioteca  carpeta_nueva  documento    fotos        mi_directorio  proyecto_final  proyectos_copia  secretos
README.md              archivos_temporales  carpeta1    codigo         documentos   lleno        mi_practica    proyectos       respaldo         videos
archivo_existente.txt  backup               carpeta2    destino        documentos2  mi_Proyecto  música         proyectos2      respaldos

