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