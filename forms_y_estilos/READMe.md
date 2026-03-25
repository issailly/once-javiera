# Bitácora de Desarrollo: Formulario de Soporte de 99 noches en el bosque

En esta etapa del proyecto, me enfoqué en la estructura inicial y la validación de los campos principales del formulario de contacto.

### 1. Organización del Proyecto
Lo primero fue poner orden en el espacio de trabajo. Creé una carpeta principal llamada `forms-y-estilos`, donde separé todo por categorías:
* **HTML:** Para la estructura del formulario.
* **Estilos:** Para toda la personalización visual.
* **README:** Con la documentación básica del proceso.

### 2. Estructura y Datos del Usuario
Configuré los campos esenciales para identificar a quien escribe. Ajusté el código para que el usuario pueda ingresar su **nombre** y su **correo electrónico** de forma clara. También personalicé la sección de **asuntos**, adaptando los temas de ayuda a las necesidades reales que se buscan cubrir.

### 3. Validación de Edad
Implementé un control estricto en el campo de edad:
* **Rango:** Solo se aceptan ingresos entre **13 y 99 años**.
* **Restricciones:** El campo está configurado como tipo numérico, por lo que bloquea automáticamente el uso de letras o caracteres especiales.

### 4. Diseño y Estilos (CSS)
Le di una identidad visual más definida al soporte:
* **Encabezado:** Cambié el color del título "Soporte de 99 noches en el bosque" a un **naranja claro** para que resalte.
* **Botón de envío:** Ahora es de color **negro**, y añadí un efecto visual para que, al seleccionarlo, el texto pase a **negrita**, dando un feedback claro al usuario de que está interactuando con él.