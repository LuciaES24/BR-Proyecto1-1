author: Lucía Espinosa Sánchez
summary: Codelab en el que se explica paso a paso cóm bastionar la BIOS en Windows
id: 1
categories: BIOS,Windows
environments: Web
status: Published

# Configuración segura de la BIOS en Windows

## 1. Introducción
Duration: 0:02:00

En este CodeLab aprenderemos a configurar nuestra BIOS de forma segura en Windows, configurando contraseñas de administración, de usuario o gestionando permisos de arranque entre otras medidas.

![Foto introducción BIOS](/pictures/bios.jpg)

¿Estas preparad@ para empezar? ¡Vamos allá!

## 2. Acceso a la BIOS
Duration: 00:04:00

Primero deberemos acceder a la BIOS de nuestro ordenador, para ello deberemos tener nuestro equipo apagado. A continuación lo encenderemos e inmediatamente comenzaremos a pulsar una tecla, cada sistema utiliza una distinta pero las más comunes son F10, F2, F12, F1 o SUPR. Posiblemente este paso no salga a la primera así que, ¡ten paciencia!.

Una vez hayamos conseguido acceder a la BIOS nos aparecerá una pantalla similar a esta:

![Foto inicio configuración BIOS](/pictures/bios_config.jpg)

A continuación comenzaremos con la configuración. ¡Vamos a empezar!

## 3. Contraseña de administrador
Duration: 00:05:00

Para comenzar con la configuración de la BIOS designaremos una contraseña de administración, la cual se solicitará para modificar parámetros de la BIOS una vez esté activada. Para activarla accederemos al panel de "Securiry", donde elegiremos la opción "Administrator Password".

![Foto configuración de seguridad BIOS](/pictures/security_config_AP.jpg)

Nos aparecerá la siguiente pantalla en la que tendremos que poner nuestra nueva contraseña de administrador.

![Foto contraseña administrador](/pictures/administrator_password.jpg)

Poco a poco vamos teniendo nuestra BIOS más segura, ¡vamos a seguir!.

## 4. Contraseña de usuario
Duration: 00:05:00

A continuación vamos a designar una contraseña de usuario, la cual tiene un funcionamiento similar a la de administrador ya que nos la solicitarán para modificar algunos parámetros básicos de la BIOS. Para ello, desde la pantalla de "Security" elegiremos la opción "User Password". 

![Foto configuración de seguridad BIOS](/pictures/security_config_AP.jpg)

Veremos una pantalla similar a la de la contraseña de administrador en la que tendremos que poner la nueva contrasela de usuario.

![Foto contraseña de usuario](/pictures/security_config_UP.jpg)

Ya tendremos las contraseñas preparadas, continuemos.

## 5. Contraseña de arranque
Duration: 00:03:00

En este apartado vamos a configurar la contraseña de arranque, la cual se nos pedirá cada vez que encendamos el disositivo. Para ello accederemos de nuevo a la pantalla "Security" y elegiremos la opción "Password Check" que por defecto estará en "Setup".

![Foto configuración de seguridad BIOS](/pictures/security_config_PC.jpg)

Una vez ahí cambiaremos la opción a "Always" para que cada vez que encendamos el dispositivo tengamos que poner la contraseña como se ve en la siguiente imagen.

![Foto contraseña de arranque](/pictures/password_check.jpg)

En el siguiente paso veremos algunos permisos.

## 6. Permiso para el arranque desde USB
Duration: 00:03:00

Si queremos controlar el arranque de nuestro ordenador para que no pueda realizarse desde un USB este apartado es primordial.
Para controlar esto accederemos al menú "Advanced" para modificar estos permisos.
Una vez ahí, las opciones que vemos señaladas en la siguiente imagen deberemos desabilitarlas, ¡y así de sencillo es!.

![Foto permisos USB](/pictures/USB_power.jpg)

¡Continuemos!

## 7. Orden de arranque
Duration: 00:07:00

Con esta configuración podremos manejar el orden de arranque de nuestro ordenador, en el que irá buscando los dispositivos indicados en orden para intentar arrancar el sistema, pasando al siguiente si uno no lo encuentra.
Para configurar esto, accederemos al menú "Boot", y en el apartado "FIXED BOOT ORDER Priorities" podremos designar los dispositivos en el orden que veamos conveniente.

![Foto orden de arranque](/pictures/boot_order.jpg)

Ya falta poco para terminar la configuración, ¡vamos allá!.

## 8. Secure Boot
Duration: 00:07:00

El arranque seguro fue introducido por Microsoft a partir de Windows 8 en el que prohíbe el arranque de cualquier otra cosa que no sea Windows aunque algunas distribuciones de Linux se han adaptado para que la ejecución pueda realizarse. 
Para configurar el arranque seguro vamos a volver a la pantalla de "Security", en la que elegiremos la opción "Secure Boot".

![Foto configuración arranque seguro](/pictures/security_config_SB.jpg)

Una vez ahí activaremos la opción de "Secure Boot".

![Foto arranque seguro](/pictures/secure_boot.jpg)

Sólo falta el último paso, ¡vamos a ello!.

## 9. Trusted computing
Duration: 00:04:00

Finalmente activaremos el TPM del ordenador, que es un chip que viene instalado en la placa base del ordenador, el cual almacena las claves de cifrado de Windows para proteger la privacidad de archivos sensibles. 

![Foto configuración TPM](/pictures/security_config_TC.jpg)

Una vez ahí activaremos la opción "Security Device Support".

![Foto TPM](/pictures/trusted_computing.jpg)


Y esta habría sido la configuración necesaria para que tu BIOS esté protegida. ¡Muchas gracias por seguir este CodeLab y espero que te haya servido!