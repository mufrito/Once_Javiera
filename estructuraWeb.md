# Resumen de la Clase 8 de CS50x

### trabajo de:
Alejandro Bolívar Echeverri.
Sámuel Díaz Sánchez.

## 1.¿como funciona internet?

En el internet nosotros tenemos un identificador único por dispositivo a esto se le llama IP (dado en notación decimal). El TPC es un protocolo que le permite a los dispositivos saber que servicio recibe y envía, ademas permite que halla múltiples dispositivos pidiendo un servicio. Algo muy importante tenemos un sistema que nos traduce los sitios para que se legible para  el dispositivo(DNS), o sea su dominio. Lo siguiente es  llamado DHCP, ello nos permite tener un registro del IP y DNS de un dispositivo para navegar sin la necesidad de dar especificaciones cada vez que accedamos a un servicio.

## 2.Protocolo HTTP y la Web.

Existe una estructura básica para las urls siendo lo mas distinguible el dominio que usualmente vemos como .com (dominio comercial): El orden correcto siento HTTPS (indica que es un sitio web encriptado) www(World Wide Web permite acceder a archivos de todo el mundo).Ejemplo.com (nombre completo del dominio).
Es en que lenguaje recibe y se envía solicitudes de paginas web( HTTP), hay otro que hace exactamente lo mismo pero con unas ligeras diferencias la mas importante que esta encriptado y la segunda que admite mayores puertos (HTTPS).
GET es una herramienta que se usa para localizar un http y permite acceder al sitio web que le envian.
200 es el codigo que le dice al navegador que esta todo bien y que puede muestrar el contenido de este.
301 le dice al servidor que a donde intenta acceder no esta disponible y que redireccione a la nueva direccion.
404 el sitio web ya no exite o se a cometido un error en la solicitud.
500 me indica que el servidor a fallado.