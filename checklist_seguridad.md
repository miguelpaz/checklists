Checklist de seguridad web
==========

En este documento se entrega una serie de elementos que deben ser revisados para determinar si un sitio web cumple con las características de seguridad mínimas.

* ¿El Sitio funciona correctamente y no presenta fallas al navegar por sus páginas o utilizar sus servicios? (especialmente en el caso de Trámites en línea)
*	Los datos ingresados por un usuario a través de formularios, ¿son validados antes de ser enviados y procesados por el servidor del Sitio?
*	¿Todos los vínculos del Sitio tienen una página asociada y el contenido adecuado al vínculo señalado?
*	Frente a una búsqueda dentro del Sitio o cualquier operación en el mismo ¿los resultados se muestran correctamente?
*	¿Los datos privados, entregados voluntariamente por los usuarios, son guardados de manera reservada?
*	¿Se ofrece una Política de Privacidad de los Datos Personales y se informa de su existencia en las páginas pertinentes?
*	¿Los servicios ofrecidos son realizados a través de canales de transacción seguros?
*	¿En los temas que requieren de accesos restringidos, el Sitio provee algún medio para validar el acceso, por ejemplo: a través de una caja de conexión con nombre de usuario y password?
*	¿La política de seguridad implementada para validar el acceso restringido es adecuada a los propósitos del servicio o de la institución?
*	¿Protege la integridad de sus programas y datos?
*	¿Se evita que sea visto, el nombre de los programas y los directorios?
*	¿Se cuenta con un protocolo de seguridad para evitar ataques externos e intrusiones de hackers?
*	¿Se cuenta con una política de respaldo de información que permita superar efectos de fallas derivadas del punto anterior?
*	¿Se ha realizado validación de inputs del usuario en el servidor?
*	¿Se ha revisado el saneamiento en el output de contenidos ingresados por usuarios?
*	¿Se ha revisado si los sitios web que requieran login de usuarios usan conexiones encriptadas vía HTTPS?
*	¿Se ha revisado si las contraseñas en el servidor son almacenadas utilizando un hash con un salt aleatorio?
*	¿Se ha verificado lógica de permisos para realizar las distintas acciones en el sitio web. Ej: Que usuarios pueden borrar, crear, editar los diferentes elementos.?
*	¿Se han filtrado los ataques de SQL Injection?. Se recomienda utilizar PreparedStatements/Consultas parametrizadas para hacer consultas a la base de datos.
*	¿Se han filtrado los ataques XSS?. Existen variadas librerias que filtran el ingreso de scripts por parte del usuario
*	¿Se han tomado medidas para prevenir los ataques XSRF/CSRF?. Las acciones del usuario sobre el sitio web deben ser enviadas vía POST, además de enviar un secret token generado al momento de presentar el formulario web.
*	¿En cuanto a la seguridad de CMS (Joomla, Wordpress, Drupal u otros): Se ha verificado que estén instalados los últimos parches de seguridad de estos sistemas?
*	¿En cuanto a la seguridad Apache / IIS / NGINX u otros : Se ha verificado que estén instalados los últimos parches de seguridad de estos servidores y verificar que las versiones en producción sean su “versión estable”?
*	¿Se han realizado respaldos de la base de datos en forma periódica o se han programado estos respaldos en tareas ?