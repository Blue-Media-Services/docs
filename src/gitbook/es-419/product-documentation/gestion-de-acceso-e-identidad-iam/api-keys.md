---
description: Learn more about API Keys and how to integrate them with our platform.
---

# Claves API

Las Claves API te permiten otorgar acceso a una API a tu cuenta de BMS. Esto facilitará el seguimiento de tus métricas utilizando una plataforma externa. Algunas APIs, como Zapier, pueden configurarse para crear Anuncios basados en archivos de Google Drive. Cuando se trata de APIs, hay mucho que podemos hacer, y cada una tendrá sus particularidades. Sin embargo, la integración de estas APIs con la consola de BMS es similar. Este artículo tiene como objetivo ayudarte a realizar esta integración.

## Gestión de Claves API

Las Claves API están disponibles en la página de permisos. Para acceder a ella, haz clic en el nombre de tu cuenta en la esquina superior derecha, luego haz clic en Permisos y, en el menú de la izquierda, selecciona Claves API.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-10-08 092211.png" alt=""><figcaption><p>Lista de Claves API</p></figcaption></figure>

### Creación de una Clave API

It is possible to [Create New API Keys](api-keys.md#create-new-api-keys) and it is also possible to [Link an Existing API Key](api-keys.md#link-existing-api-key).

#### Crear nuevas Claves API

1. Haz clic en <img src="../../.gitbook/assets/image (9) (1).png" alt="" data-size="line"> para agregar una Clave API.
2.  Selecciona Crear Clave API y luego completa los detalles.

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-08 100509.png" alt=""><figcaption><p>Editor de Claves API</p></figcaption></figure>

    * Nombre: Asigna un nombre a tu Clave API.
    * Etiquetas: Asigna etiquetas para tu organización.
    * Políticas: Configura las políticas de acceso que limitan a qué da acceso esta Clave API; haz clic en <img src="../../.gitbook/assets/image (22).png" alt="" data-size="original"> para agregar tus políticas. Cada política tiene un nombre y una descripción de lo que permite acceder. También puedes crear la Clave API sin seleccionar una política.

    <figure><img src="../../.gitbook/assets/image (978) (1).png" alt=""><figcaption><p>Modal de Selección de Políticas</p></figcaption></figure>

    * Después de seleccionar todas las políticas necesarias, haz clic en <img src="../../.gitbook/assets/image (153).png" alt="" data-size="line"> para confirmar tu selección.
3. Haz clic en <img src="../../.gitbook/assets/image (24) (1).png" alt="" data-size="line"> para guardar tu Clave API.

#### Vincular Clave API Existente

Esta opción te permite vincular una Clave API existente de otra cuenta de BMS.

{% hint style="info" %}
Al vincular una Clave API existente, otorgarás acceso a tu cuenta a los usuarios de la Clave API vinculada. Utiliza las políticas para controlar lo que se puede hacer a través de esta Clave API.
{% endhint %}

1. Haz clic en <img src="../../.gitbook/assets/image (9) (1).png" alt="" data-size="line"> para agregar una Clave API.
2.  Selecciona **Vincular Clave API existente** y luego completa los detalles.

    <figure><img src="../../.gitbook/assets/image (948).png" alt=""><figcaption><p>Vinculación de una API Existente</p></figcaption></figure>

    * ID de Clave API: Ingresa el ID de la Clave API que deseas vincular.
    * Políticas: Configura las políticas de acceso que limitan a qué da acceso esta Clave API haciendo clic en <img src="../../.gitbook/assets/image (22).png" alt="" data-size="original"> para agregar tus políticas. Cada política requiere un nombre y una descripción del acceso que proporciona. Al vincular Claves API, se debe seleccionar al menos una política.
    * Después de seleccionar todas las políticas necesarias, haz clic en <img src="../../.gitbook/assets/image (153).png" alt="" data-size="line"> para confirmar tu selección.
3. Haz clic en <img src="../../.gitbook/assets/image (24) (1).png" alt="" data-size="line"> para guardar tu Clave API.

### Pestaña de Códigos de Acceso

Después de crear la Clave API, necesitas generar un Código de Acceso antes de poder empezar a usarla. Si seleccionas una Clave API vinculada, esta pestaña permanecerá deshabilitada, ya que no es necesario crear un código de acceso. En esos casos, usarás el Código de Acceso de la API vinculada, que puede ser proporcionado por su creador.

<figure><img src="../../.gitbook/assets/image (155).png" alt=""><figcaption><p>Pestaña de Códigos de Acceso</p></figcaption></figure>

1. Selecciona la Clave API para la cual se debe crear el código de acceso.
2.  Haz clic en <img src="../../.gitbook/assets/image (156).png" alt="" data-size="line"> para crear un código de acceso para la Clave API seleccionada.\\

    <figure><img src="../../.gitbook/assets/image (149).png" alt=""><figcaption><p>Creación de Código de Acceso</p></figcaption></figure>
3. Ingresa una descripción para tu código de acceso.
4. Haz clic en <img src="../../.gitbook/assets/image (157).png" alt="" data-size="line"> para guardar tu código de acceso.
5.  Justo después de guardar tus cambios, se mostrará el secreto del código de acceso de la siguiente manera:

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-09 090427.png" alt=""><figcaption><p>Secreto del Código de Acceso</p></figcaption></figure>
6. Es posible copiar el secreto usando el botón de copiar, <img src="../../.gitbook/assets/image (419).png" alt="" data-size="original"> , o descargarlo en un archivo '.txt'.

Puedes crear hasta 2 códigos de acceso por Clave API; cada código es válido por 365 días. Recomendamos encarecidamente crear un nuevo código unas semanas antes de que el código actual expire para garantizar que los servicios que dependen de esta Clave API no se interrumpan.

### Cómo acceder a BMS a través de la API

Para interactuar con los servicios de BMS de manera programática, necesitas incluir el Código de Acceso generado en tus solicitudes API. Tu acceso estará restringido a las APIs específicas que tu Clave API está autorizada a usar. Puedes incluir el Código de Acceso en tus solicitudes usando uno de los siguientes métodos:

*   **En el Encabezado de Solicitud:** Copia el "x-api-key" usando el botón <img src="../../.gitbook/assets/image (985).png" alt="" data-size="original"> . Esto evitará errores de tipeo, y pégalo en el encabezado de tus solicitudes.

    <figure><img src="../../.gitbook/assets/image (984).png" alt=""><figcaption><p>Acceso a BMS a través de la API - Método del Encabezado de Solicitud</p></figcaption></figure>
*   **En la Cadena de Consulta:** Agrega el Código de Acceso a la URL como un parámetro de consulta apiKey. También puedes usar el botón de copiar para evitar errores de tipeo.

    <figure><img src="../../.gitbook/assets/image (986).png" alt=""><figcaption><p>Acceso a BMS a través de la API - Método de la Cadena de Consulta</p></figcaption></figure>

Para una lista completa de las APIs de BMS disponibles, por favor consulta nuestra [documentación](https://api.bluems.com/).

### Edición de Claves API y Códigos de Acceso

Todos los detalles de las Claves API están disponibles para edición haciendo clic en <img src="../../.gitbook/assets/image (420).png" alt="" data-size="line"> en la misma fila de la Clave API que deseas editar. Después de realizar tus cambios, haz clic en <img src="../../.gitbook/assets/image (421) (1).png" alt="" data-size="line"> para guardarlos.

También puedes eliminar una Clave API haciendo clic en <img src="../../.gitbook/assets/image (422) (1).png" alt="" data-size="original"> , y luego confirmando la acción en <img src="../../.gitbook/assets/image (423) (1).png" alt="" data-size="line">. Ten cuidado: esta acción no se puede deshacer. Ten en cuenta que cualquier API que dependa de la Clave API eliminada dejará de funcionar.

Con respecto a los Códigos de Acceso, puedes ver el secreto del código de acceso y descargar las credenciales haciendo clic en <img src="../../.gitbook/assets/image (424) (1).png" alt="" data-size="original"> en la misma fila del código de acceso que deseas ver. La descripción del código de acceso también se puede editar haciendo clic en <img src="../../.gitbook/assets/image (420).png" alt="" data-size="line"> en la misma fila del código de acceso que deseas modificar. Una vez que hayas terminado de realizar tus cambios, haz clic en <img src="../../.gitbook/assets/image (421) (1).png" alt="" data-size="line"> para guardarlos.

{% hint style="danger" %}
¡Atención! Ten cuidado al eliminar un código de acceso, esta acción no se puede deshacer y todos los servicios que dependen de este código dejarán de funcionar.
{% endhint %}

También puedes eliminar códigos de acceso. Esto es útil en casos donde los datos podrían haber sido comprometidos. Para hacerlo, primero desactiva el código apagando el interruptor a la derecha del código de acceso <img src="../../.gitbook/assets/image (425) (1).png" alt="" data-size="original">, luego haz clic en <img src="../../.gitbook/assets/image (422) (1).png" alt="" data-size="original"> en la misma fila del código de acceso que deseas eliminar y confirma haciendo clic en <img src="../../.gitbook/assets/image (423) (1).png" alt="" data-size="line">.
