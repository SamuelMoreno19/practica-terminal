# practica-terminal
Ejercicio practico - leccion #1
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