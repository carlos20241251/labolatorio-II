# labolatorio-II
bashtop  y  gestion de repositoro 
Actualize los repositorios del sistema (update & Upgrade)

sudo apt update && sudo apt upgrade -y
 los repositorios actualmente en
 grep -r ^deb /etc/apt/sources.list /etc/apt/sources.list.d/
/


Instale la herramienta "Bashtop Resource Monitor" en caso de ser necesario, agregarla al repositorio local 
apt-cache search bashtop

sudo apt install bashtop
cdc



Una vez halla presentado la herramienta anterior, proceda a desinstalarla. eliminando tambien todos los archivos de configuracion

sudo apt purge bashtop -y


Elimine todas las dependencias asociadas a este programa que ya no esten en uso

cd 
ls
sudo apt autoremove -y
rm -rf bashtop
ls 

# CREACION DE TAREA Y ACTUALIZACION 

sudo crontab -e
 
0 23 * * * apt update && apt upgrade -y
 ctrl  + x para guardar 

Programe su máquina para que se reinicie todos los domingos a las 3 a.m.

sudo crontab -e

0 3 * * 0 /sbin/reboot
ctrl + x
Cree una tarea programada usando el comando "at" para que elimine el contenido de la carpeta /tmp dentro de 1 minuto. Mostrar el resultado con ls /tmp antes y despues de la ejecucion
ls /tmp

at now + 1 minute
rm -rf /tmp/*
Ctrl + D
ls /tmp

#PRACTICA  3
lsblk

#crear la particion 

sudo fdisk /dev/nvme0l
n
p
enter
enter
w

#formatear en ext4
sudo mkfs.ext4 /dev/nvme0l

#crear carpeta de escritorio
cd 
mkdir disco20GB

 montar la particion 

#sudo mount /dev/nvme01ls ~/Escritorio/disco20GB

comprobar
 df -h

#crear el archivo 
cd ~/home/lavoe/disco20GB
touch AdrianAlcantara.txt
ls

#desmontar la unidad
sudo umount ~/home/lavoel/disco20GB

#montar en /mnt
sudo mount /dev/sdb1 /mnt
 
verificar el archivo 
cd /mnt
ls

