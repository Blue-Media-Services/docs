# Cookie Pools

Un Cookie Pool es una recopilación o base de datos de las cookies de los usuarios. Las cookies son pequeños fragmentos de datos que se almacenan en el navegador web de un usuario cuando visita un sitio web. Estas cookies registran el comportamiento en línea de los usuarios, sus preferencias y sus interacciones con los sitios web y los servicios.

En el contexto de la publicidad y el marketing digitales, un Cookie Pool puede tener varios fines:

* **Segmentación de la audiencia:** Segmenta a los usuarios en diferentes grupos según sus intereses, comportamientos, datos demográficos u otros criterios. Esta segmentación permite realizar campañas publicitarias más específicas y personalizadas.
* **Retargeting:** Recopila datos de los usuarios basados en eventos y acciones con fines de seguimiento. Estos datos se pueden utilizar posteriormente para crear modelos de recomendación para tus campañas de retargeting, mejorando así tus conversiones. [Obtenga más información sobre las Campañas de Retargeting](../../solutions/retargeting.md).
* **Personalización de anuncios:** Utilice los datos recopilados para mostrar anuncios más relevantes para cada usuario de su público objetivo, basándose en su actividad reciente en línea, sus intereses y su comportamiento. Los anuncios personalizados son más atractivos y permiten al anunciante obtener mejores resultados.
* **Análisis y medición:** Realice un seguimiento del rendimiento de sus campañas, midiendo las tasas de clics, las tasas de conversión y la participación de los usuarios, entre otras métricas.&#x20;
* **Límite de frecuencia:** Establezca límites de frecuencia para restringir la cantidad de veces que se muestra un anuncio concreto a un usuario en un determinado periodo de tiempo. Esto evita que se muestre el mismo anuncio al mismo usuario repetidamente.&#x20;

## Gestión de Cookie Pools

<figure><img src="../../.gitbook/assets/Captura de tela 2025-07-02 095105.png" alt=""><figcaption><p>Lista de Cookie Pools</p></figcaption></figure>

### Crear un Cookie Pool

Un cookie pool debe crearse poco antes de utilizarlo para una campaña, de modo que pueda rellenarse. Configure cuánto tiempo deben estar disponibles sus cookies antes de caducar, establezca cuántas cookies desea almacenar en su pool y seleccione los Ad Exchanges que utilizará para sincronizar sus cookies con él.

1. Haga clic en ![Create Cookie Pool](<../../.gitbook/assets/image (1049).png>) para crear un cookie pool.
2.  Rellene los datos:

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-15 090606.png" alt=""><figcaption><p>Editor de Cookie Pool</p></figcaption></figure>

    * Nombre: Introduzca un nombre para su cookie pool.
    * Etiquetas: Introduzca las etiquetas correspondientes a su organización.
    * Exchanges: Seleccionar ad exchanges para sincronizar con tus cookies, te recomendamos seleccionar solo los exchanges que vas a utilizar para ejecutar tus campañas publicitarias, con el fin de evitar cargos innecesarios.
    * TTL: Establece el número de días que una cookie se mantendrá en el pool después de la sincronización.
    * Tamaño máximo: Establece la cantidad máxima de cookies que se almacenarán. Una vez alcanzado el límite, no se añadirán más cookies al pool hasta que caduquen las antiguas, pero las cookies recopiladas seguirán estando disponibles para su uso. También es posible aumentar el tamaño máximo para permitir que se recopilen más cookies.
3. Haga clic en ![Save](<../../.gitbook/assets/image (1046).png>) para guardar tu Cookie Pool.

### Edición de un Cookie Pool

Después de crear un cookie pool, puedes editarlo haciendo clic en el botón de edición <img src="../../.gitbook/assets/image (64).png" alt="editing button" data-size="line">. Todos los parámetros son editables. En el caso del TTL, los cambios solo se aplicarán a las cookies recién añadidas. Después de realizar los cambios, haga clic en ![Save](<../../.gitbook/assets/image (1046).png>) para salvarlos.

Es posible archivar cookie pools para una mejor organización. Haga clic en ![](<../../.gitbook/assets/image (273).png>) archivar los seleccionados cookie pools, visualiza tus archivos cookie pools activando el interruptor "Archivado" situado encima del cookie pools lista. También es posible desarchivar un cookie pool haciendo clic en ![](<../../.gitbook/assets/image (274).png>).

### Eliminar un Cookie Pool

{% hint style="danger" %}
¡Atención! Ten cuidado al eliminar cookie pools, esta acción no se puede deshacer y todos los datos relacionados, incluidas las métricas recopiladas anteriormente, también se eliminarán.
{% endhint %}

Puedes eliminar un cookie pool haciendo clic en el botón eliminar <img src="../../.gitbook/assets/image (65).png" alt="delete button" data-size="original">, se le mostrará una advertencia indicando que esta acción no se puede deshacer. Para continuar con el proceso, haga clic en ![Delete](<../../.gitbook/assets/image (1048).png>) para confirmar que lo estás eliminando y ya está. Ten en cuenta que los objetivos basados en estos cookie pools dejará de funcionar.

## Instalación de un Cookie Pool

Después de crear un cookie pool deberá instalarlo en su sitio web para comenzar a utilizarlo. Para ello, siga las instrucciones que se indican en la pestaña "Instrucciones de instalación" de la Cookie Pools página.

<figure><img src="../../.gitbook/assets/image (67).png" alt=""><figcaption><p>Pestaña Instrucciones de Instalación</p></figcaption></figure>

1. Seleccione el cookie pool lo instalará marcando la casilla de verificación situada junto a su nombre.
2. En la pestaña Instrucciones de instalación, haga clic en <img src="../../.gitbook/assets/image (68).png" alt="" data-size="line"> para copiar el código.
3. Pega el código lo más arriba posible dentro de la etiqueta \<head> de la página.
4. Si lo desea, es posible utilizar un identificador de usuario único, lo cual resulta útil si sus usuarios inician sesión en varios dispositivos. Para ello, descomente la parte indicada del código e inserte el identificador de usuario único.

También puede utilizar un administrador de etiquetas, como Google Tag Manager (GTM), para añadir este código a su sitio web.

## Pestaña Métricas

Después de instalar su cookie pools deberías empezar a recibir datos de ellos. Es posible seguir este proceso en la pestaña de métricas. Estas son las métricas disponibles para cookie pools:

* [Recuento de Vencimientos](dmp-metrics.md#expiration-count)
* [Tamaño Máximo](dmp-metrics.md#max-size)
* [Tamaño](dmp-metrics.md#size)
* [Recuento de Sincronización](dmp-metrics.md#sync-count)
* [Tiempo hasta el Vencimiento](dmp-metrics.md#time-until-expiration)
