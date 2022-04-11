# Guila de instalacion para Hyper y Oh my zsh 
 instalar las terminales zsh y oh-my-zsh en Windows

# Paso 1


# Paso 2
abrir "configuración"


![imagen](https://user-images.githubusercontent.com/6835007/162633516-00463a30-da52-464f-b6ba-2c1346418bec.png)

habilitar modo desarrollador

![imagen](https://user-images.githubusercontent.com/6835007/162633664-3ad69a91-bc53-40b2-8b70-201c2954c155.png)

en caso que solicite reinicio lo podemos hacer

# Paso 3
Habilitar Windows Subsystem Linux desde el panel de control

Clic en Programas 

![imagen](https://user-images.githubusercontent.com/6835007/162633727-29186481-0b67-4f60-b6a0-103562af4ffc.png)

Clic en Activar o desactivar las características de Windows

![imagen](https://user-images.githubusercontent.com/6835007/162633736-868b087a-1a18-4a78-84d1-e835889cd357.png)

habilitar el subsistema para linux

![imagen](https://user-images.githubusercontent.com/6835007/162633773-3f3b3454-c5a2-449c-beb7-cdbd0e7b9089.png)



# Paso 4
Desde Microsoft store buscamos e instalamos Ubuntu

![imagen](https://user-images.githubusercontent.com/6835007/162633812-a0bdeefb-90bf-423e-9ebb-518f6d9839f3.png)



# Paso 5
Abrir ubuntu y configurar nombre y contraseña


![imagen](https://user-images.githubusercontent.com/6835007/162746562-9f843db1-4036-46cb-8b29-ebc9d5d3a7e5.png)



# Paso 6
Instalar ZSH y Oh-my-zsh

sudo apt-get update  


sudo apt-get install zsh


y ahora instalar zsh



curl -Lo install.sh https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh



sh install.sh


# Paso 7
Definir ZSH como terminal por defecto

chsh -s /usr/bin/zsh


Muchas veces eso no es suficiente, por lo que le tenemos que indicar al archivo de configuración (.bashrc) la terminal que debe de ejecutar y para eso, realizamos los siguientes pasos:

    Ejecutamos el siguiente comando: nano ~/.bashrc
    En la parte superior del archivo agregamos las siguientes líneas:

if test -t 1; then
exec zsh
fi

y luego nuevamente ejecutamos


chsh -s /usr/bin/zsh



# Paso 8
descargar e instalar hyper 

https://hyper.is/#installation

abrir hyper y buscamos las preferencias


![imagen](https://user-images.githubusercontent.com/6835007/162634528-89df9e8f-4508-4a87-a7fe-40f2e2382307.png)

![imagen](https://user-images.githubusercontent.com/6835007/162634670-bbcafec2-26d5-42cf-959d-21feee280e55.png)

colocamos en shell la siguiente linea para que quede por defecto


Fuente: https://platzi.com/blog/como-instalar-zsh-en-windows/


# Bonus
Si quieres cambiar el tema
https://github.com/ohmyzsh/ohmyzsh/wiki/Themes

abre

nano ~/.zshrc

y buscas THEME



