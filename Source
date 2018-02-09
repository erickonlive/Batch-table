@ECHO off
SET "B=%random%"
SET "EID=100000000000000"
SET "P=Main\fn.dll sprite"
main\fn.dll font 8
mode 48,15
%P% 0 20 C "!Atencion!"
%P% 3 0 C "Para el correcto funcionamiento de la aplicacion"
%P% 5 7 C "Cambie el idioma de su"&%P% 5 30 9F "facebook"
%P% 7 3 C "A cualquier"&%P% 7 15 A Ingles&%P% 7 22 c "en su listado de idiomas"
%P% 14 0 5F "Precione una tecla para continuar"
pause>nul 
mode 34,6
SET /a vare=0 + 0
setlocal enabledelayedexpansion enableextensions
main\fn.dll font 7
IF EXIST main\nircmd.exe (SET "nir=main\nircmd infobox") ELSE (SET "nir=ECHO. ")
IF EXIST main\fart.exe (goto down) ELSE (!NIR! "Falta Fart.exe, El programa no se puede ejecutar" "Error 5")
pause>nul
exit
:down
IF EXIST main\fn.dll (goto ill) ELSE (!NIR! "Falta fn.dll, El programa no se puede ejecutar" "Error 3")
exit
:ill
Title F-Viewer - !UN!

main\fn.dll cursor 0
:menu
endlocal
setlocal enabledelayedexpansion enableextensions
cls
color A
!P! 01 06 !B! "Buscar por ID"
!P! 02 06 !B! "Buscar todos los post"
!P! 03 06 !B! "Obtener ID unico"
!P! 00 00 C "**********************************"
!P! 04 00 C "**********************************"
!P! 02 33 C "*"
!P! 01 33 C "*"
!P! 03 33 C "*"
!P! 01 00 C "*"&!P! 01 06 A "Buscar por ID"
!P! 02 00 C "*"&!P! 02 06 A "Buscar todos los post"
!P! 03 00 C "*"&!P! 03 06 A "Obtener ID unico"

!P! 01 03 !B! "1"
!P! 02 03 !B! "2"
!P! 03 03 !B! "3"
!P! 01 02 F "-1-"
!P! 02 02 F "-2-"
!P! 03 02 F "-3-"
ECHO.
ECHO.
ECHO.
ECHO.
ECHO.
SET /p dol=-
if /i "!dol!"=="1" Goto ID1
if /i "!dol!"=="2" Goto EX
if /i "!dol!"=="3" Goto graph
if /i "!dol!"=="" !NIR! "Este campo no puede estar vacio" "Error"&goto menu
if /i "!dol!"=="!dol!" !NIR! "Opcion invalida" "Error"
goto menu
:ID1
cls
color F
!P! 01 06 !B! "ID previamente guardado"
!P! 02 06 !B! "Ingresar ID"
!P! 03 06 !B! "Regresar"
!P! 00 00 9 "**********************************"
!P! 04 00 9 "**********************************"
!P! 02 33 9 "*"
!P! 01 33 9 "*"
!P! 03 33 9 "*"
!P! 04 00 9 "**********************************"
!P! 01 00 9 "*"&!P! 01 06 F "ID previamente guardado"
!P! 02 00 9 "*"&!P! 02 06 F "Ingresar ID"
!P! 03 00 9 "*"&!P! 03 06 F "Regresar"

!P! 01 03 !B! "1"
!P! 02 03 !B! "2"
!P! 03 03 !B! "3"
!P! 01 02 F "-1-"
!P! 02 02 F "-2-"
!P! 03 02 F "-3-"
ECHO.
ECHO.
ECHO.
ECHO.
ECHO.
SET /p VARL=:
if /i "!VARL!"=="1" (goto ttre)
if /i "!VARL!"=="2" (goto SETid)
if /i "!VARL!"=="" !NIR! "Este campo no puede estar vacio" "Error"&goto menu
if /i "!VARL!"=="3" cls&goto menu
if /i "!VARL!"=="!VARL!" !NIR! "Opcion invalida" "Error"
:ttre
cls
ECHO Nombre del ID guardado:
SET /p IDV=:
IF EXIST PSN\!IDV!.bat (call PSN\!IDV!.bat&goto ID2) ELSE (goto ID1)
cls
:SETid
cls
ECHO Escriba el ID
SET /p ID=:
:ID2
Title F-Viewer - !IDV!
cls
SET "PO=https://www.facebook.com/search/!ID!/photos-of"
SET "FB=https://www.facebook.com/search/!ID!/photos-by"
SET "L=https://www.facebook.com/search/!ID!/photos-liked"
SET "POR=https://www.facebook.com/search/!ID!/photos-of/intersect"
SET "CP=https://www.facebook.com/search/!ID!/photos-commented"
SET "LP=https://www.facebook.com/search/!ID!/pages-liked"
SET "G=https://www.facebook.com/search/!ID!/groups"
SET "LMP=https://www.facebook.com/search/!ID!/photos-liked/last-month/date/photos/intersect"
SET "PPP=https://graph.facebook.com/!ID!/picture?width=!ID!
if !vare!==49 goto men2
:down2
SET /a vare=0
SET /a vares=0
cls
SET /a vare=!vare! + 34
SET /a vares=!vares! + 6
:xy
SET /a vare=!vare! + 1
SET /a vares=!vares! + 1
mode !vare!,!vares!
if !vares!==15 (goto ru2) ELSE (goto ru2)
:ru2
if !vare!==49 (goto men2) ELSE (goto xy)
:men2
cls
ECHO ------------------------------------------------
ECHO -1 Fotos de                                    -
ECHO -2 Fotos por                                   -
ECHO -3 Fotos que le gustan                         -
ECHO -4 Etiquetadas y likeadas                      -
ECHO -5 Fotos en las que comento                    -
ECHO -6 Paginas que le gustan                       -
ECHO -7 Grupos                                      -
ECHO -8 Ultimas fotos del mes                       -
ECHO -9 Ver foto de perfil (                      ) -
ECHO -10 Ver amistad con                            -
ECHO ------------------------------------------------
ECHO -11 probar con otra persona                    -
ECHO -12 regresar el menu                           -
ECHO ------------------------------------------------
!P! 09 23 C "Use "GETP" y descargarla"
!P! 20 10 F "Aplicacion escrita por:"
!P! 20 34 9 "Erick Antonio"
SET /p OP=:
if /i "!OP!"=="1" start !PO!&goto ID2
if /i "!OP!"=="2" start !FB!&goto ID2
if /i "!OP!"=="3" start !L!&goto ID2
if /i "!OP!"=="4" start !POR!&goto ID2
if /i "!OP!"=="5" start !CP!&goto ID2
if /i "!OP!"=="6" start !LP!&goto ID2
if /i "!OP!"=="7" start !G!&goto ID2
if /i "!OP!"=="9" start !PPP!&goto ID2
if /i "!OP!"=="10" goto FS
if /i "!OP!"=="11" goto id1
if /i "!OP!"=="8" start !LMP!&goto ID2
if /i "!OP!"=="GETP" goto wget
if /i "!OP!"=="SVP" goto svprofrile
if /i "!OP!"=="12" goto resuse
if /i "!OP!"=="" !NIR! "Porfavor escoje una opcion antes de precionar enter" "Error"&goto ID2
if /i "!OP!"=="!OP!" !nir! "Opcion invalida" "Error"&goto ID2
:FS
cls
ECHO escriba el id o el nombre de usuario de la segunda persona:
SET /p fp=:
cls
ECHO generando link...
timeout 2
start https://www.facebook.com/!ID!?and=!fp!
cls
goto men2
:svprofrile
CLS
cls
ECHO escriba un nombre para guardar:
SET /p UN=-
IF EXIST PSN\!UN!.bat (Nircmd infobox "Este perfil ya esta registrado"&goto men2) ELSE (goto bump)
:bump
CLS
IF NOT EXIST PSN MD PSN
ECHO guardando perfil...
(
ECHO.@ECHO off
ECHO.SET "UN=!UN!"
ECHO.SET "ID=!ID!"
ECHO.SET "UN=!UN!"
ECHO.goto men2
)>PSN\!UN!.bat
goto men2
:ex
cls
ECHO primer nombre de la victima en facebook
SET /p FN=:
cls
ECHO segundo nombre de la victima
ECHO !FN!
SET /p LN=:
cls 
ECHO !FN! !LN!
copy /y ht\resq.html >NUL 2>NUL
main\fart "resq.html" BLink !FN! >NUL 2>NUL
main\fart "resq.html" Bl1nk !LN! >NUL 2>NUL
ECHO cargando...
SET "B=!B!"
ren resq.html !FN!!LN!.html
MD PG >NUL 2>NUL
move !FN!!LN!.html PG\ >NUL 2>NUL 
start PG\!FN!!LN!.html
goto menu
:graph
SET /a vare=0
SET /a vares=0
cls
SET /a vare=!vare! + 34
SET /a vares=!vares! + 6
:ru3
if !vares!==10 (goto ru4) ELSE (SET /a vares=!vares! + 1)
:ru4
mode !vare!,!vares!
if !vare!==55 (goto men3) ELSE (SET /a vare=!vare! + 1)
goto ru3
:men3
cls
ECHO introdusca el nombre de usuario de la persona, Ejemplo:
!P! 01 00 F "https://facebook.com/"
!P! 01 21 C "Nombre.usuario"
!p! 01 35 F "?fref=nf"
ECHO.
ECHO.
ECHO Pegue el Nombre de usuario aqui:
main\fn.dll cursor 1
SET /p UN=: 
IF /i "!UN!"=="" (Nircmd infobox "El campo esta vacio" "Error"&goto men3) ELSE (goto ddr3)
:ddr3
cls
ECHO Obteniendo informacion de !UN! 
main\wget -o log.x00 graph.facebook.com/!UN! >NUL 2>NUL
Title F-Viewer - !UN!
IF EXIST !UN! (type !UN!&goto 3) ELSE (!nir! "A ocurrido un error, estas conectado a internet?" "Error 6"&goto men3)
:3
!P! 05 10 F "Escriba los numeros que estan entre comillas "
SET /p ID=Escriba el ID que se muestra arriba:
echo.
echo.
echo.
echo.
IF "!ID!" LSS "!EID!" (main\nircmd infobox "El ID es incorrecto" "Error")
del !UN!
cls
goto down2
) ELSE (goto here)
:here
del !UN!
goto id2
copy /y ht\resq1.html >NUL 2>NUL
main\fart "resq1.html" BLink !FN! >NUL 2>NUL
ECHO cargando...
SET "B=%B%"
ren resq.html !FN!!LN!.html
MD PG >NUL 2>NUL
move !FN!!LN!.html PG\ >NUL 2>NUL 
goto ID2
:resuse
SET /a vare=49
SET /a vares=15
:big
mode !vare!,!vares!
if !vare!==34 (goto menu) ELSE (SET /a vare=!vare! - 1&goto no)
:no
if !vares!==6 (goto big) ELSE (SET /a vares=!vares! - 1&goto big)
:wget
ECHO Espera...
IF NOT EXIST foto md foto
IF NOT EXIST FOTO\!UN! MD FOTO\!UN!
main\wget -r -c -k -nd --no-check-certificate graph.facebook.com/!ID!/picture?width=10000000 >NUL 2>NUL
ren *.JPG@OH* !UN!~%B%.jpg >NUL 2>NUL
move /y *.jpg* foto\!UN!\ >NUL 2>NUL
IF EXIST UlIqmHJn-SK.gif del UlIqmHJn-SK.gif & NIRCMD INFOBOX "El usuario no existe o ha desactivado su cuenta" "Error"&goto menu
IF NOT EXIST foto\!UN!\!UN!~%B%.jpg NIRCMD INFOBOX "No se ha podido conectar." "Error de red"&goto men2
start foto\!UN!\!UN!~%B%.jpg
Title F-Viewer - !UN!
goto men2
