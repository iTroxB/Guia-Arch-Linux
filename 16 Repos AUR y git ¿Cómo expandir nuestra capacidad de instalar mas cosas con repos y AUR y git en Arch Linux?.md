# 17 Repos y AUR ¿Cómo expandir nuestra capacidad de instalar mas cosas con repos y AUR en Arch Linux?

Paso 1: Instalamos con pacman git, le damos a enter, con la tecla enter del teclado

    pacman -S git

seguido de

    pacman -S wget

Paso 2: Le decimso que si, escribiendo "y"

    y

Paso 3: Entramos con nuestro usuario, asi que salimos:

    exit

Paso 4: En nuestro usuario, en desktop creamos una carpeta que se llame repos:

    mkdir -p Desktop/hagrid/repos

Paso 5: Entramos en la carpeta repos:

    cd !$

Paso 6: instalamos aur:

    git clone https://aur.archlinux.org/paru-bin.git

Paso 7: Entramos dentro para ejecutarlo:

    cd paru-bin

Paso 8: Ejecutamos ESTE PASO, que sirve para cualquier repo de aur o que contenga archivo PKGBUILD, es un comando que te ayudará en adelante

    makepkg -si
    
Si te diera error:

     ==> ERROR: Cannot find the fakeroot binary.
     
Debes de usar el siguiente comando:

     sudo pacman -S --needed base-devel
   
Y esto instalará los paquetes necesarios, y luego ejecutas el paso 8.

Paso 9: Introducimos la contraseña y escribimos "y"

    y

### Pequeño paréntesis: primero: git clone y el link, a veces acabad en git! PASO 6! Y luego cd a la carpeta, seguido de makepkg -si

Paso 10: OPCIONAL ahora no: Para instalar archivos que nos descarguemos .deb instalamos con yay:

    yay -S debtap

Paso 11 OPCIONAL ahora no: Con usuario sudo ejecutamos en la carpeta:

    debtap -u /lugar/del/archivo.deb

Paso 12: Instalamos node

    sudo pacman -Sy nodejs

Paso 13: Para el futuro, no hacer: Borramos si teniamos Node

    sudo pacman -Rsc -n nodejs

Paso 14: Para finalizar:

    sudo pacman -Sy npm

Paso 15: Ejecutamos por si acaso:

    pacman -Syu

Paso 16: Comprobamos que se ha instalado:

    node -v

Paso 17: Comprobamos npm

    npm -v

Paso 18: Instalar pnpm

    wget https://get.pnpm.io/install.sh | sh

seguido de:

    chmod +x ./install.sh

y de:

    ./install.sh

Paso 19: Seguido del comando source

    source /home/TuNombreDeUsuario/.bashrc
    
Paso 20: Instalar Yarn para repos de React

    pacman -S yarn


Siguiente capítulo:

[17 Interfaz grafica ¿Cómo instalar la interfaz grafica en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/17%20Interfaz%20grafica%20%C2%BFC%C3%B3mo%20instalar%20la%20interfaz%20grafica%20en%20Arch%20Linux%3F.md) 🔵

Volver al capítulo anterior:

[15 Internet ¿Cómo añadir internet a la máquina en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/15%20Internet%20%C2%BFC%C3%B3mo%20a%C3%B1adir%20internet%20a%20la%20m%C3%A1quina%20en%20Arch%20Linux%3F.md) ✅

Volver al Índice:

[00 Readme o Índice](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux)


 - Esto es lo que has hecho: ✅
 - Tu estás aquí: 💙
 - Esto es lo que te falta por leer: 🔵

[00 Readme o Índice](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux) ✅

[01 Descarga Linux Arch - Guia Definitiva Arch Linux](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/01%20Descarga%20Arch%20Linux%20%C2%BFC%C3%B3mo%20descargar%20Arch%20Linux%3F.md) ✅

[02 Montar el USB con Rufus ¿Cómo montar usb booteable con rufus para instalar Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/02%20Montar%20el%20USB%20con%20Rufus%20%C2%BFC%C3%B3mo%20montar%20usb%20booteable%20con%20rufus%20para%20instalar%20Arch%20Linux%3F.md) ✅

[03 Preriquisitos de BIOS ¿Cómo quitar Intel Rapid Start Technology?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/03%20Preriquisitos%20de%20BIOS%20%C2%BFC%C3%B3mo%20quitar%20Intel%20(r)%20Rapid%20Start%20Technology%3F.md) ✅

[04 Discos y particiones ¿Cómo particionar el disco para Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/04%20Discos%20y%20particiones%20%C2%BFC%C3%B3mo%20particionar%20el%20disco%20para%20Arch%20Linux%3F.md) ✅

[05 Montar particiones ¿Cómo montar particiones y directorios en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/05%20Montar%20particiones%20%C2%BFC%C3%B3mo%20montar%20particiones%20y%20directorios%20en%20Arch%20Linux%3F.md) ✅

[06 Contraseñas ¿Cómo poner contraseñas en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/06%20Contrase%C3%B1as%20%C2%BFC%C3%B3mo%20poner%20contrase%C3%B1as%20en%20Arch%20Linux%3F.md) ✅

[07 Usuarios y Grupos ¿Cómo crear usuarios en grupos en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/07%20Usuarios%20y%20Grupos%20%C2%BFC%C3%B3mo%20crear%20usuarios%20en%20grupos%20en%20Arch%20Linux%3F.md) ✅

[08 Idiomas ¿Cómo añadir mi idioma?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/08%20Idiomas%20%C2%BFC%C3%B3mo%20a%C3%B1adir%20mi%20idioma%3F.md) ✅

[09 Instalar Bootloader ¿Cómo instalar el bootloader en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/09%20Instalar%20Bootloader%20%C2%BFC%C3%B3mo%20instalar%20el%20bootloader%20en%20Arch%20Linux%3F.md) ✅

[10 Configurar grub ¿Cómo configurar el archivo de configuración para grub?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/10%20Configurar%20grub%20%C2%BFC%C3%B3mo%20configurar%20el%20archivo%20de%20configuraci%C3%B3n%20para%20grub%3F.md) ✅

[11 Hostname ¿Cómo añadir nuestro propio hostname a la máquina?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/11%20Hostname%20%C2%BFC%C3%B3mo%20a%C3%B1adir%20nuestro%20propio%20hostname%20a%20la%20m%C3%A1quina%3F.md) ✅

[12 Región y Hora ¿Cómo asignar tu región y hora?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/12%20Regi%C3%B3n%20y%20Hora%20%C2%BFC%C3%B3mo%20asignar%20tu%20regi%C3%B3n%20y%20hora%3F.md) ✅

[13 Instalar neofetch ¿Cómo instalar neofetch en tu Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/13%20Instalar%20neofetch%20%C2%BFC%C3%B3mo%20instalar%20neofetch%20en%20tu%20Arch%20Linux%3F.md) ✅

[14 Login Arch Linux ¿Cómo hacer log in en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/14%20Login%20Arch%20Linux%20%C2%BFC%C3%B3mo%20hacer%20log%20in%20en%20Arch%20Linux%3F.md) ✅

[15 Internet ¿Cómo añadir internet a la máquina en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/15%20Internet%20%C2%BFC%C3%B3mo%20a%C3%B1adir%20internet%20a%20la%20m%C3%A1quina%20en%20Arch%20Linux%3F.md) ✅

[16 Repos AUR y git ¿Cómo expandir nuestra capacidad de instalar mas cosas con repos y AUR y git en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/16%20Repos%20AUR%20y%20git%20%C2%BFC%C3%B3mo%20expandir%20nuestra%20capacidad%20de%20instalar%20mas%20cosas%20con%20repos%20y%20AUR%20y%20git%20en%20Arch%20Linux%3F.md) 💙

[17 Interfaz grafica ¿Cómo instalar la interfaz grafica en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/17%20Interfaz%20grafica%20%C2%BFC%C3%B3mo%20instalar%20la%20interfaz%20grafica%20en%20Arch%20Linux%3F.md) 🔵

[18 Instalar Blackarch ¿Cómo instalar herramientas de blackarch en nuestro arch linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/18%20Instalar%20Blackarch%20%C2%BFC%C3%B3mo%20instalar%20herramientas%20de%20blackarch%20en%20nuestro%20arch%20linux%3F.md) 🔵

[19 Instalar rust ¿Cómo instalar rust, cargo y bottom en arch linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/19%20Instalar%20rust%20%C2%BFC%C3%B3mo%20instalar%20rust%2C%20cargo%20y%20bottom%20en%20arch%20linux%3F.md) 🔵

[20 Instalar Snap Store ¿Cómo instalar Snap Store en arch linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/20%20Instalar%20Snap%20Store%20%C2%BFC%C3%B3mo%20instalar%20Snap%20Store%20en%20arch%20linux%3F.md) 🔵

[21 Qmake OpenGL ¿Cómo instalar qmake para comilar opengl en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/21%20Qmake%20OpenGL%20%C2%BFC%C3%B3mo%20instalar%20qmake%20para%20comilar%20opengl%20en%20Arch%20Linux%3F.md) 🔵

[22 Docker, Instala docker en arch linux](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/22%20Docker%2C%20Instala%20docker%20en%20Arch%20Linux.md) 🔵

[23 Postgresql, ¿Cómo instalar Postgresql en Arch Linux](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/23%20Postgresql%2C%20%C2%BFC%C3%B3mo%20instalar%20Postgresql%20en%20Arch%20Linux%3F.md) 🔵

[24 Instalar Anaconda 3](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/24%20Anaconda%203%2C%20%C2%BFC%C3%B3mo%20instalar%20Anaconda%203%20en%20Arch%20Linux%3F.md) 🔵

[95 Alias, Comandos ¿Cómo ser un mago y ejecutar comandos en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/95%20Alias%2C%20Comandos%20%C2%BFC%C3%B3mo%20ser%20un%20mago%20y%20ejecutar%20comandos%20en%20Arch%20Linux%3F.md) 🔵

[96 MOTD de bienvenida en Arch Linux?](https://github.com/miguelgargallo/Guia-Definitiva-Arch-Linux/blob/main/96%20MOTD%20de%20bienvenida%20en%20Arch%20Linux%3F.md) 🔵

Espero que te haya gustado este capítulo de la Guia Definitiva Arch Linux, si es así dame un follow en [twitter](https://twitter.com/miguelgargallo) para apoyarme! Fork y Fav a esta repo!
