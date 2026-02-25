# Rastreadores

Los rastreadores son pequeños scripts que se colocan en el código de su sitio web para recopilar datos sobre las actividades de sus usuarios. A continuación, podemos utilizar los datos recopilados para crear modelos de recomendación con los que llevar a cabo campañas de retargeting y mejorar sus conversiones. Además, estos datos pueden proporcionar información valiosa sobre los intereses de sus usuarios, lo que facilita la creación de campañas publicitarias más eficaces.&#x20;

## **Gestión de Rastreadores**

<figure><img src="../../../.gitbook/assets/Captura de tela 2024-12-05 074113.png" alt=""><figcaption><p>Lista de Rastreadores</p></figcaption></figure>

### Creación de un Rastreador

Los Rastreadores recopilarán datos sobre las actividades de su sitio web, por lo que deben estar instalados y activos durante un tiempo antes de que sus datos puedan utilizarse para una campaña.

1. Haga clic en <img src="../../../.gitbook/assets/image (269).png" alt="" data-size="line"> para empezar a crear un Rastreador.
2.  Rellene los datos:

    <figure><img src="../../../.gitbook/assets/image (1034).png" alt=""><figcaption><p>Editor de Rastreadores</p></figcaption></figure>

    * Nombre: Establezca un nombre para su rastreador.
    * Etiquetas: Establezca etiquetas para su organización.
    * Número máximo de usuarios: Establezca el número máximo de usuarios que se deben rastrear. Una vez alcanzado el límite, no se añadirán más usuarios nuevos al rastreador, pero los usuarios añadidos seguirán siendo rastreados.
    * Máximo de eventos por usuario: Establezca el número máximo de eventos por usuario que se deben rastrear. Una vez alcanzado el límite, la recepción de nuevos eventos provocará que los más antiguos caduquen.
    * Antigüedad máxima de la actividad: Establezca el número de días durante los que se almacenarán los datos de los usuarios rastreados. Transcurrido este periodo, los datos se eliminarán.
3. Haga clic en <img src="../../../.gitbook/assets/image (93) (1) (1).png" alt="" data-size="line"> para guardar tu rastreador.

### Edición de un Rastreador

Todos los parámetros de los rastreadores son editables, haga clic en ![](<../../../.gitbook/assets/image (272).png>) en la misma fila del rastreador que desea editar, realice los cambios y, a continuación, haga clic en ![Save](<../../../.gitbook/assets/image (1046).png>) para salvarlos.

Es posible archivar los rastreadores para una mejor organización. Haga clic en ![](<../../../.gitbook/assets/image (273).png>) para archivar el rastreador seleccionado, visualice sus rastreadores archivados activando el interruptor "Archivado" situado encima de la lista de rastreadores. También es posible desarchivar un rastreador haciendo clic en ![](<../../../.gitbook/assets/image (274).png>).

### Eliminar un Rastreador

También podemos eliminar nuestros rastreadores haciendo clic en el botón eliminar. ![](<../../../.gitbook/assets/image (275).png>) en la misma fila que el rastreador que desea eliminar y, a continuación, confirmándolo haciendo clic en ![Delete](<../../../.gitbook/assets/image (1048).png>). Esta acción no se puede deshacer, así que ten cuidado. Además, ten en cuenta que los modelos de recomendación basados en el rastreador eliminado podrían dejar de funcionar.

{% hint style="danger" %}
_¡Atención! Ten cuidado al eliminar rastreadores, ya que esta acción no se puede deshacer y todos los datos relacionados, incluidas las métricas recopiladas anteriormente, también se eliminarán._
{% endhint %}

## Gestión de Eventos y Acciones

Configure los eventos que se deben rastrear y las acciones que debe realizar el rastreador cuando se produzca el evento.

<figure><img src="../../../.gitbook/assets/image (100).png" alt=""><figcaption><p>Pestaña Configuración de los Rastreadores</p></figcaption></figure>

### Creación de eventos y acciones

Configura eventos según las actividades que realizan los usuarios en tu sitio web o aplicación, por ejemplo, añadir productos al carrito, ver productos y otras.

1. En la pestaña Configuración, haga clic en <img src="../../../.gitbook/assets/image (278).png" alt="" data-size="original"> para empezar a crear un evento.
2. Rellene los datos:

<figure><img src="../../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Editor de Eventos</p></figcaption></figure>

* Nombre: Establezca un nombre para su evento.
* ID del evento: Establezca un ID para su evento, si no se establece ningún ID, se utilizará el nombre del evento como ID predeterminado.
* Campos de datos personalizados: Establezca los campos de datos personalizados que se recopilarán cuando se capture el evento.
* Moneda: Utilice este campo para especificar la referencia monetaria del evento. Debe reflejar la moneda utilizada en su sitio web. Ayuda a realizar un seguimiento del valor monetario asociado a la acción del usuario.
* Importe: Este campo captura la cantidad asociada al evento. Por ejemplo, en un evento de compra, representa el número de productos comprados en una sola transacción. Declare una variable en su sitio web que refleje este importe.
* ID de deduplicación: Este campo se utiliza para asignar un identificador único a cada instancia de evento. Garantiza que los eventos duplicados no se cuenten varias veces, lo que mejora la fiabilidad de los datos.
* Plantilla: La opción de plantilla está disponible para todos los campos anteriores. Define cómo se procesarán los valores del evento. Acepta una cadena que utiliza variables de los campos de datos personalizados y genera una salida separada por comas.&#x20;

1. Haga clic en ![](<../../../.gitbook/assets/image (278).png>) para añadir una acción a tu evento, la acción es lo que tu rastreador hará en BMS una vez que el usuario acceda a la página diseñada o realice la acción especificada.
2. Rellene los datos:
   * Nombre: Establezca un nombre para su acción.
   *   ¿Qué hacer?:

       <figure><img src="../../../.gitbook/assets/Captura de tela 2025-02-27 084243.png" alt=""><figcaption><p>Editor de acciones</p></figcaption></figure>

       *   Seguimiento en el Catálogo: Le permite realizar un seguimiento de los eventos basándose en un catálogo de productos.

           * Catálogo: Seleccione el catálogo que desea utilizar.
           * Seguir como: Seleccione esta acción, ya que debe ser seguida.
           * Campo que contiene los ID de oferta: Seleccione el campo personalizado que contiene el ID de oferta o utilice una plantilla.
           * Plantilla: Inserte una plantilla específica que se utilizará para crear una lista separada por comas de los ID de oferta que se van a rastrear.
           * Datos personalizados disponibles: Los campos de datos personalizados configurados en su evento se mostrarán aquí para ayudarle a crear una plantilla.

           <figure><img src="../../../.gitbook/assets/Captura de tela 2025-02-27 084528.png" alt=""><figcaption><p>Editor de acciones</p></figcaption></figure>
       * Rastreador de Identifier Pool: Esta opción le permite añadir o eliminar identifiers de sus pools.
         * Identifier Pool: Seleccione el identifier pool enlazarás con esta acción.
         * Operación: Seleccione si desea añadir o eliminar identifiers de sus pools.
3. Haga clic en <img src="../../../.gitbook/assets/image (93) (1) (1).png" alt="" data-size="line"> para guardar tu acción.
4. Siéntete libre de agregar más acciones a este evento y cuando hayas terminado, haz clic en <img src="../../../.gitbook/assets/image (93) (1) (1).png" alt="" data-size="line"> para guardar tu evento.

### Edición de eventos y acciones

Edita tus eventos y acciones para satisfacer las necesidades de tu negocio.

Podemos editar eventos haciendo clic en ![](<../../../.gitbook/assets/image (272).png>) en la misma fila del evento que se va a editar en la pestaña Configuración, todos los parámetros de los eventos están disponibles para ser editados. Una vez finalizados los cambios, haga clic en ![Save](<../../../.gitbook/assets/image (1046).png>) para salvarlos.

Los parámetros de las acciones también se pueden editar. Para ello, busca el evento que contiene la acción que deseas editar en la pestaña Configuración y haz clic en ![](<../../../.gitbook/assets/image (272).png>) en la misma fila del evento y, a continuación, haciendo clic en ![](<../../../.gitbook/assets/image (272).png>) en la misma fila de la acción que desea editar, realice los cambios y haga clic en ![Save](<../../../.gitbook/assets/image (1046).png>) para guardar los cambios, haga clic en ![Save](<../../../.gitbook/assets/image (1046).png>) vuelve a guardar los cambios realizados en el evento y ya está.

También es posible duplicar eventos y acciones haciendo clic en ![](<../../../.gitbook/assets/image (366).png>) en la misma fila del evento o acción que necesita duplicar. Esta función puede ser útil si necesita crear una nueva acción o evento manteniendo algunos parámetros de uno ya existente.

### Eliminación de eventos y acciones

Es posible eliminar eventos y acciones haciendo clic en ![](<../../../.gitbook/assets/image (275).png>) en la misma fila del evento o acción que desea eliminar y, a continuación, confirme la acción haciendo clic en ![Delete](<../../../.gitbook/assets/image (1048).png>). Esta acción no se puede deshacer, así que ten cuidado al realizarla. Como alternativa, también es posible desactivar eventos y acciones cambiando la posición del interruptor de <img src="../../../.gitbook/assets/image (89) (1) (1).png" alt="" data-size="original"> a ![](<../../../.gitbook/assets/image (90) (1) (1).png>) en la misma fila del evento o acción que desea desactivar.

## Instrucciones de Instalación

Después de configurar los eventos y acciones para tu rastreador, debes instalarlo en tu sitio web. Para ello, sigue las instrucciones que se indican en la pestaña Instrucciones de instalación. Consulta nuestra [Instrucciones de Instalación](install-instructions.md) artículo para obtener más información sobre nuestros métodos de instalación.

## Pestaña Métricas

Después de instalar los rastreadores, debería empezar a recibir datos de ellos. Es posible seguir este proceso en la pestaña de métricas; estas son las métricas disponibles para los rastreadores:

* [Recuento de Ejecución de Acciones](../dmp-metrics.md#action-execution-count)
* [Tasa de Fallos de Acciones](../dmp-metrics.md#action-failure-rate)
* [Recuento de Actividades](../dmp-metrics.md#activity-count)
* [Valor de la Actividad](../dmp-metrics.md#activity-value)
* [Recuento de Vencimientos](../dmp-metrics.md#expiration-count-1)
* [Máximo de Usuarios](../dmp-metrics.md#maximum-users)
* [Tiempo hasta el Vencimiento](../dmp-metrics.md#time-until-expiration-1)
* [Recuento de usuarios del Rastreador](../dmp-metrics.md#tracker-user-count)
