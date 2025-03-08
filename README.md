# creador-cuentas-autom-tico-de-Crunchyroll
Notas e instrucciones:

Correo temporal: El código genera un correo temporal utilizando un servicio como Mailinator. Si deseas usar otro servicio, puedes modificar la función get_temp_email().

Generación de contraseñas seguras: La función generate_password() crea contraseñas seguras utilizando una combinación de letras, números y caracteres especiales. Puedes ajustar la longitud si lo prefieres.

Guardado de cuentas en archivo: Si la cuenta se crea correctamente, los datos de la cuenta se guardan en un archivo cuentas_creadas.txt. Asegúrate de tener permisos para escribir en el archivo en la ubicación donde ejecutas el script.

Configuración del navegador: El código utiliza undetected_chromedriver para iniciar un navegador Chrome sin problemas de detección. Asegúrate de tener este paquete instalado y actualizado.

Verificación de la creación de la cuenta: El código verifica si la cuenta se ha creado correctamente buscando un mensaje de verificación en la página web. Si no se encuentra, se registrará un error.

Control de errores y cierre del navegador: El navegador se cierra correctamente al final, incluso si ocurren errores. El bloque finally asegura que driver.quit() se ejecute para cerrar el navegador.

Personalización de la URL: Actualmente, el formulario de registro está configurado para la URL de Crunchyroll. Si deseas usar este código para otra página, debes modificar la URL en la función fill_registration_form().
