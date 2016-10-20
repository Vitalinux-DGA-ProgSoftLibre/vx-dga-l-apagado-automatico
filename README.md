# Paquete DEB vx-dga-l-apagado-automático

Paquete encargado de poder programar un hora u horas de apagado para el equipo Linux.
Para el control del momento del apagado se hace uso de cron y la gestión de permisos mediante sudo.
Mediante diferentes *.desktop se posibilita el poder habilitar nuevas horas de apagado, reconfigurar el apagado o poder comprobar las horas de apagado programadas.

# Usuarios Destinatarios

Usuarios que quieren configurar un apagado de manera automatizada para su equipo Linux

# Aspectos Interesantes:
```
Ninguno a resaltar
```
# Como Crear el paquete DEB a partir del codigo de GitHub
Para crear el paquete DEB será necesario encontrarse dentro del directorio donde localizan los directorios que componen el paquete.  Una vez allí, se ejecutará el siguiente comando (es necesario tener instalados los paquetes apt-get install debhelper devscripts):

```
apt-get install debhelper devscripts
/usr/bin/debuild --no-tgz-check -us -uc
```

# Como Instalar el paquete generado vx-dga-l-*.deb:
Para la instalación de paquetes que estan en el equipo local puede hacerse uso de ***dpkg*** o de ***gdebi***, siendo este último el más aconsejado para que se instalen también las dependencias correspondientes.
```
gdebi vx-dga-l-*.deb
```
