README


-Congelador de archivos en Linux para la carpeta /home/$USER. 

El cometido de este script es no guardar cambios realizados en la carpeta del usuario, así cualquier archivo o carpeta que el usuario cree se borraran automaticamente al apagar el ordenador.
Tambien afecta a la configurción del navegador restaurando la configuración deseada enn cada inicio de sesión nuevo.

Como funciona.
-Consiste en hacer una copia de la carpeta $USER cada vez que apliquemos un cambio en la configuración y que se deba guardar para una optimización o simplemente control del uso para los usuarios establecidos.

-Con el comando desde consola:   

   sudo fijausuario $USER 

-Se creara una copia en /srv/$USER que se guarda para el proximo inicio de sesión.

-Cada vez que se reinicia el equipo se ejecuta un comando que repone la carpeta   del usuario desde /srv/$USER hacia /home/$USER borrando todos los cambios que se   han hecho durante la sesion en la carpeta del $USER.


