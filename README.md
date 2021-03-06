# DuckyKatzJS - Payloads de USB Rubber Ducky usando katz.js

<img align="right" src="./cuac.jpeg">

**duckykatz2gmail:** Este payload se encargará de descargar mediante powershell el JScript katz.js de subTee (https://gist.githubusercontent.com/subTee/b30e0bcc7645c790fcd993cfd0ad622f/raw/2adcc9d2570b4367c6cc405e5a5969863d04fc9b/katz.js), ejecutarlo y enviarnos a través de Gmail el archivo .log con la información de Mimikatz.

**duckykatz2txtoffline:** Este payload se encargará de ejecutar el JScript katz.js de subTee que se encuentra en la memoria SD de nuestro Rubber Ducky, el payload iniciará un bucle hasta encontrar el volumen de la memoria que contenga el "katz.js" que nosotros hemos introducido anteriormente, lo ejecutará y guardará la información extraida en un archivo TXT dentro de la memoria SD. **Para usar este payload se necesita tener la versión Twin Ducky Firmware flasheada en el Rubber Ducky.** 

## Como flashear Rubber Ducky a Twin Ducky Firmware

* Primero lo que necesitaremos es una terminal de Linux para ejecutar el siguiente comando:
  
  > apt-get install dfu-programmer
  
* Luego descargaremos ducky-flasher y los descomprimiremos con los siguiente comandos:

  > wget https://github.com/hak5darren/USB-Rubber-Ducky/raw/master/Flash/ducky-flasher1.0.zip                  
  > unzip ducky-flasher1.0.zip
  
* Ahora instalaremos la herramienta y la ejecutaremos:

  > cd ducky-flasher                                                                                            
  > sudo python setup.py                                                                                                             
  > sudo ducky-flasher

* A continuación deberemos conectar el Rubber Ducky en modo DFU, para ello lo insertaremos en el puerto USB a la vez que mantenemos pulsado el boton que tiene en la parte superior.

* Cuando lo hayamos conectado, en el programa elegimos la opción "Twin Duck" presionando el número 4, luego elegimos la versión original presionando el número 1 y esperamos a que el programa acabe de flashear nuestro Rubber Ducky.
