+++
title = 'Códigos HTTP'
date = 2023-09-14T16:51:30Z
draft = false  
+++

## El protocolo HTTP. Códigos

Los códigos de respuesta HTTP se utilizan para indicar el estado de la solicitud realizada al servidor. Estos códigos están agrupados en cinco clases, según el primer dígito del código:

### 1xx: Información
- `100 Continue`: El servidor ha recibido los encabezados de la solicitud y el cliente debería proceder a enviar el cuerpo de la solicitud.
- `101 Switching Protocols`: El servidor está cambiando a un protocolo diferente, que ha sido solicitado por el cliente.

### 2xx: Éxito
- `200 OK`: La solicitud fue exitosa y el servidor responde con el recurso solicitado.
- `201 Created`: La solicitud ha resultado en la creación de un nuevo recurso.
- `204 No Content`: La solicitud fue exitosa pero no hay información para enviar de vuelta (por ejemplo, en una solicitud DELETE).

### 3xx: Redirección
- `300 Multiple Choices`: Hay múltiples opciones que un cliente puede seguir.
- `301 Moved Permanently`: El recurso ha sido movido de forma permanente a una nueva ubicación.
- `302 Found`: El recurso se encuentra temporalmente en una ubicación diferente.
- `304 Not Modified`: El recurso no ha sido modificado y el cliente debería usar su copia en caché.

### 4xx: Errores del Cliente
- `400 Bad Request`: La solicitud es inválida o no puede ser procesada por el servidor.
- `401 Unauthorized`: La solicitud requiere autenticación.
- `403 Forbidden`: El cliente no tiene permisos para acceder al recurso.
- `404 Not Found`: El recurso solicitado no se encuentra en el servidor.
- `405 Method Not Allowed`: El método HTTP utilizado no está permitido para este recurso.

### 5xx: Errores del Servidor
- `500 Internal Server Error`: Un error genérico cuando falla una operación en el servidor.
- `501 Not Implemented`: El servidor no soporta la funcionalidad necesaria para cumplir la solicitud.
- `502 Bad Gateway`: Un servidor intermedio ha recibido una respuesta inválida desde otro servidor.
- `503 Service Unavailable`: El servidor no puede manejar la solicitud, generalmente porque está sobrecargado o en mantenimiento.

Estos son solo algunos de los códigos de estado HTTP más comunes. Cada uno tiene su propio significado y proporciona información útil tanto para el cliente como para los desarrolladores.