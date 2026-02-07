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
