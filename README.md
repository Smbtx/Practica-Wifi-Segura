CIBERSEGURIDAD

Modulo 6 – Seguridad Web y conectividad

Alumno: Gomez David Gabriel.

Comisión: 90870

Informe de Auditoria de Red Wi-Fi Insegura



**Practica-Wifi-Segura**



En este trabajo se analiza el comportamiento de la navegación mediante el protocolo HTTP en una red, con el fin de identificar los riesgos de seguridad al transmitir información sin cifrado y comprender como debemos protegernos.





**PARTE 1 - EXPLORACION:**



**URL solicitada**:silvershinningfreshmorning.neverssl.com/online/

**Método HTTP:** HTTP/1.1

**Host:** neverssl.com (dirección asignada: silvershinningfreshmorning.neverssl.com)

**Protocolo utilizado:** HTTP/1.1 (Sin cifrado).

**Headers enviados (cabeceras visibles)**: Toda la información viaja en texto plano, incluyendo datos del navegador, sistema operativo y tipo de conexión.



**Sitio analizado:** 

Dirección: HTTP://neverssl.com

Característica: Sitio diseñado para funcionar exclusivamente por HTTP, sin cifrado SSL/ TLS.





**PARTE 2 - ANALISIS**



**evidencia observada:**

**¿Qué protocolo utiliza el sitio?**

Al inspeccionar las solicitudes desde las herramientas de desarrollador (F12 pestaña de red) Se observa que el protocolo utilizado es HTTP/1.1 Puedo confirmar esto porque el navegador indica el aviso "Not Secure".



**¿Qué información puede observarse durante la solicitud?**



Durante la solicitud pueden observarse; 

Host: neverssl.com

URL:silvershinningfreshmorning.neverssl.com/online/

Método GET: GET

User-agent: Mozilla/5.0 (X11; Linux x86\_64; rv:130.0) Gecko/20100101 Firefox/130.0

Headers: 

Host: neverssl.com — identifica el sitio al que se accede

User-Agent: revela el navegador, su versión y el sistema operativo

Accept: indica los tipos de contenido admitidos

Connection: define el tipo de conexión establecida





Riesgos encontrados:

**3. ¿Qué riesgos existen al navegar mediante HTTP desde una red Wi-Fi pública?**

Al navegar por HTTP en una red Wi-Fi pública nos encontramos con los siguientes riesgos:

Cualquier persona en la misma red puede ver qué sitios visite,

&#x20;Puede leer todo lo que envío y recibo: contraseñas, mensajes, formularios,

&#x20;Puede modificar el contenido de la página en tránsito,

&#x20;Puede redirigirme a sitios falsos sin que lo detecte,

&#x20;No hay privacidad ni integridad de los datos.



**4. ¿Cómo cambiaría este escenario utilizando una VPN?**

Al implementar el uso de una VPN el escenario mejora por lo siguiente:



Cifrado: Todo el tráfico se codifica desde el dispositivo, antes de salir a la red.

&#x20;Túnel seguro: Se crea una conexión protegida directamente con el servidor de la VPN.

Protección: La red pública solo ve que me conecto a la VPN, no puede ver qué sitios visito ni qué datos intercambio.

Privacidad: Incluso si visito sitios en HTTP, todo el tráfico viaja cifrado dentro del túnel.



**5. Escribe tus 3 Reglas de Oro para navegar en redes Wi-Fi públicas.**



Luego de lo que estuve estudiando sobre el tema, puedo decir con toda seguridad que mis 3 Reglas de Oro para Redes Wi-Fi Públicas

1\_Nunca ingresar contraseñas ni datos sensibles en sitios que no muestren el candado y "HTTPS" en la barra de direcciones.

2\_Siempre se debe Activar una VPN antes de conectarse a cualquier red pública (ideal tener activado el Kill Switch)

3\_ Siempre desactivar la conexión automática a redes desconocidas y no compartir archivos cuando estés fuera de casa.













