# Creativos

Las creatividades son el componente más pequeño de nuestro servidor de anuncios y representan lo que se mostrará al usuario final cuando se muestre su anuncio.

Las creatividades de display son, básicamente, bloques de código HTML. Puede proporcionar este código usted mismo o usar nuestro editor integrado para configurar una creatividad sencilla con una imagen interactiva.

## Gestión de Creativos

<figure><img src="../../.gitbook/assets/image (239).png" alt=""><figcaption><p>Lista creativa</p></figcaption></figure>

## Creación de una Creatividad

Para comenzar a crear su creatividad, haga clic en <img src="../../.gitbook/assets/image (556).png" alt="Create Creative" data-size="line">.

Complete los detalles:

<figure><img src="../../.gitbook/assets/image (542).png" alt=""><figcaption></figcaption></figure>

* Nombre - cómo desea llamar a esta creatividad;
* Etiquetas - hasta 5 etiquetas que pueden usarse para facilitar la identificación y búsqueda;
* Dominio - el dominio principal al que esta creatividad dirigirá al usuario al hacer clic;
* Tipo - el tipo de creatividad, como tamaños comunes de IAB como "Large Leaderboard (970x90)", "Banner (468x60)", etc.

Después de hacer clic en el menú desplegable disponible para seleccionar un tipo de creatividad, tendrá acceso a una lista que contiene todos los tipos que pueden usarse; estos son los tipos disponibles:

<table data-header-hidden><thead><tr><th width="408.2222900390625">Texto</th><th>Texto</th></tr></thead><tbody><tr><td>Super Leaderboard / Pushdown (970x90)</td><td>Rectángulo medio (300x250)</td></tr><tr><td>Leaderboard (728x90)</td><td>Rectángulo grande (336x280)</td></tr><tr><td>Banner (468x60)</td><td>Cuadrado pequeño (200x200)</td></tr><tr><td>Leaderboard para smartphone (320x50)</td><td>Cuadrado (250x250)</td></tr><tr><td>Banner para smartphone (300x50)</td><td>Intersticial para móvil (640x1136)</td></tr><tr><td>Banner pequeño para teléfonos básicos (120x20)</td><td>Intersticial para móvil (1080x1920)</td></tr><tr><td>Banner mediano para teléfonos básicos (168x28)</td><td>Intersticial para móvil (750x1334)</td></tr><tr><td>Banner grande para teléfonos básicos (216x36)</td><td>Media página (300x600)</td></tr><tr><td>Billboard (970x250)</td><td>Retrato (300x1050)</td></tr><tr><td>Leaderboard grande para smartphone (320x100)</td><td>Rascacielos ancho (160x600)</td></tr><tr><td>Financiero (120x60)</td><td>Rascacielos (120x600)</td></tr></tbody></table>

Para diseñar su creatividad, tiene dos opciones:

### Imagen Estática

* Para utilizar una imagen sencilla con un enlace, en la pestaña "Imagen Estática", complete lo siguiente:
  * La imagen que desea mostrar. Puede pegar la URL de una imagen que ya tenga alojada o utilizar la integración con la BMS Media Library para buscar o subir una nueva.
    * Nota: La BMS Media Library permite subir imágenes estáticas o GIFs, siempre que el tamaño del archivo sea de 2 MB o menos.
  * El enlace que desea abrir cuando se haga clic en la imagen. Puede ser cualquier URL HTTPS con cadenas de consulta (query strings) como las UTM. Se añadirá nuestro rastreador de clics estándar para mostrar las métricas de la creatividad.

### Edición de UTMs

Al insertar el enlace al sitio web designado para su creatividad, es importante configurar sus etiquetas UTM. Si no tiene sus etiquetas creadas previamente, puede utilizar <img src="../../.gitbook/assets/image (543).png" alt="Edit UTMs" data-size="line"> para realizar ajustes en su URL y ver una vista previa en tiempo real para validar su dirección. Este botón se encuentra en el espacio denominado "Enlace a". Tras hacer clic en el botón, aparecerá la pantalla de configuración de etiquetas UTM.

<figure><img src="../../.gitbook/assets/image (591).png" alt=""><figcaption><p>Editor de UTM</p></figcaption></figure>

Se le presentará la URL actual de su sitio web y, a continuación, cada etiqueta UTM con su explicación para ayudarle a completarlas.

{% hint style="warning" %}
Si no se ha informado ninguna URL, **deberá** insertar la **URL** correspondiente al dominio de su sitio web; si no se presenta ninguna URL, no será posible configurar sus UTM.
{% endhint %}

Al editar las UTM, cada vez que cambie una etiqueta, se actualizará automáticamente la URL de su enlace, mostrándole la versión actual de sus etiquetas.

*   **UTM Fuente:** Identifica la fuente del tráfico. En este caso, usaría "BMS" como su fuente.

    * **Ejemplo - "BMS":** Para saber que la creatividad proviene de la plataforma BMS.

    **Nota:** Puede añadir cualquier tipo de fuente a su UTM; depende de usted decidir cuál es mejor.
* **UTM Medio:** Puede utilizar un medio de campaña para identificar el medio en el que un visitante encontró su URL, como redes sociales, código QR, coste por clic (CPC), afiliados, anuncios orgánicos/pagados, boletines informativos, etc.
  * **Ejemplo - "Social":** Dado que la campaña se dirigirá a redes sociales, podemos establecer el medio como Social.
* **UTM Campaña:** Como su nombre indica, se utiliza para dar un nombre a su campaña, como "Rebajas de Black Friday", "Rebajas de Acción de Gracias", "Campaña de Lanzamiento", etc.
  * **Ejemplo - "SuCampaña":** Aquí puede indicar simplemente el nombre de su campaña para identificar mejor la campaña en la que se está utilizando la creatividad.
* **UTM Contenido:** El contenido de la campaña es útil cuando se realizan pruebas A/B de anuncios. Diferencia enlaces idénticos que dirigen a la misma URL. Por ejemplo, cuando tiene dos enlaces en un mismo correo electrónico, este parámetro distingue entre ellos.
  * **Ejemplo - "PaginaDeInicio":** El contenido que se le presentará al usuario; si estamos realizando pruebas A/B en diferentes páginas, esta es una forma de configurar la etiqueta UTM de contenido.
* **UTM Término:** Identifica palabras clave de pago en campañas de anuncios (se utiliza principalmente para campañas de búsqueda de pago).
  * **Ejemplo - "Zapatos Deportivos":** Esto identifica la campaña de búsqueda de pago en la que las palabras clave utilizadas fueron Zapatos Deportivos.

Una vez que configure todas sus etiquetas UTM, pulse el <img src="../../.gitbook/assets/image (546).png" alt="Save" data-size="line"> bot botón, y sus etiquetas se configurarán en consecuencia.

<figure><img src="../../.gitbook/assets/image (547).png" alt=""><figcaption><p>Etiquetas UTM configuradas</p></figcaption></figure>

### Pegar HTM

Para utilizar una creatividad totalmente personalizada, cambie a la pestaña "Pegar HTML" e inserte el código HTML final que se mostrará cuando el usuario vea su creatividad.

{% hint style="warning" %}
¡Cuidado! Se le presentarán algunas macros más adelante en esta sección. Debe utilizarlas para habilitar el seguimiento de clics de BMS en sus anuncios; de lo contrario, **no se realizará el seguimiento de los clics.**
{% endhint %}

<figure><img src="../../.gitbook/assets/image (795).png" alt=""><figcaption><p>Ejemplo de personalización de HTML</p></figcaption></figure>

Esto puede ser cualquier cosa y depende totalmente de usted producir una creatividad funcional con HTML, CSS y Javascript.

Cuando proporciona el código HTML, nuestro rastreador de clics no se añadirá automáticamente. Puede copiar la macro del rastreador de clics (o cualquier otra macro que desee) desde los botones de asistencia de plantilla en la parte inferior y pegarla en su HTML. Para obtener más información, por favor eche un vistazo a la [Sección de Macros](creatives.md#macros).

Puede utilizar la <img src="../../.gitbook/assets/preview.png" alt="Preview" data-size="line"> botón para ver cómo se mostrará su creatividad y para asegurarse de que dirija a los usuarios al sitio correcto al hacer clic.

Si está listo para enviar la creatividad a revisión, asegúrese de que la opción "Enviar para revisión" esté marcada. Si desea seguir editándola más tarde, déjela desmarcada.

Después de realizar todos los ajustes necesarios, haga clic en ![Save](<../../.gitbook/assets/image (555).png>).

#### Macros

Nuestro servidor de anuncios proporciona varias macros que pueden utilizarse dentro de su código HTML; estas se encuentran en la parte inferior de la pestaña Pegar HTML.

<figure><img src="../../.gitbook/assets/image (796).png" alt=""><figcaption><p>Sección de Macros Disponibles</p></figcaption></figure>

Algunas de ellas son:

* **Rastreadores de clics de BMS** - Estas macros permitirán que BMS rastree los clics en sus anuncios. Si no instala ninguna de estas, no se registrará ningún evento de clic ni métrica.
  * **URL de clic sin escape** \
    Esta es la versión más utilizada. Debe instalarse al principio del enlace, antes de cualquier otro rastreador y antes de la propia URL final.
  * **URL de clic con escape** \
    Esta versión es similar a la anterior, pero solo debe usarse si desea tener un rastreador de clics externo que no admita URLs sin escape.
  * **URL de clic con doble escape** \
    Esta versión es similar a las dos anteriores, pero solo debe usarse si desea tener una cadena de dos o más rastreadores de clics donde los rastreadores externos no admitan URLs sin escape.
  * **Cache Buster**\
    Esta macro inyectará una secuencia aleatoria de números y se utiliza comúnmente para garantizar que las solicitudes no se almacenen en la caché.

### Revisión de la Creatividad

Al finalizar la creación de su creatividad, esta se enviará a revisión para identificar si es inapropiada. A continuación, puede encontrar algunos de los estados que pueden mostrarse para su creatividad:

* **En cola:** La creatividad se encuentra en la cola de revisión.
* **En progreso:** La plataforma aún está revisando la creatividad.
* **Aprobada:** La creatividad ha sido aprobada sin ninguna restricción.
* **Parcialmente aprobada:** La creatividad ha sido aprobada con restricciones (regiones o plataformas específicas).
* **Rechazada:** La creatividad ha sido rechazada y no puede utilizarse.
* **Revocada:** La creatividad fue aprobada previamente, pero ha sido revocada.
* **Omitida:** El proceso de revisión fue omitido y no se ejecutó.

Si tiene alguna pregunta sobre el resultado del estado de revisión de su creatividad, póngase en contacto con nuestro equipo de soporte.

### Edición de una Creatividad

Para editar una creatividad, utilice el <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> botón en la creatividad correspondiente. Todos los campos están disponibles para edición, excepto los selectores de dominio y de tipo.

<figure><img src="../../.gitbook/assets/image (548).png" alt=""><figcaption><p>Edición de una creatividad</p></figcaption></figure>

Si modifica la URL de la imagen, el enlace o el código HTML, la creatividad volverá al <img src="../../.gitbook/assets/draft status.png" alt="Draft" data-size="line"> estado, y deberá enviar la creatividad a revisión nuevamente. Mientras esté en borrador, la creatividad no se mostrará en ninguna campaña.

Una vez que haya realizado todos los cambios necesarios en su creatividad, haga clic en ![Save](<../../.gitbook/assets/image (555).png>).

### Habilitar y deshabilitar una creatividad

![](<../../.gitbook/assets/image (154).png>)

Para que se muestre en una campaña, una creatividad debe estar habilitada. Si desea evitar que se muestre una creatividad, puede deshabilitarla y dejará de generar impresiones inmediatamente.

### Archivar y desarchivar una creatividad

Las creatividades que no se utilicen con frecuencia pueden archivarse haciendo clic en el <img src="../../.gitbook/assets/archive.png" alt="Archive" data-size="line"> botón. Archivar una creatividad no impide que sea utilizada o mostrada; simplemente la oculta de la vista principal.

Para ver todas las creatividades archivadas, simplemente active el <img src="../../.gitbook/assets/archive filter.png" alt="Archived" data-size="line"> filtro. Puede desarchivar <img src="../../.gitbook/assets/unarchive.png" alt="Unarchive" data-size="line"> una creatividad para devolverla a la lista principal.

### Eliminar una creatividad

Puede eliminar una creatividad haciendo clic en <img src="../../.gitbook/assets/delete.png" alt="Delete" data-size="line">. Si la creatividad se está utilizando, se le presentará una lista de los grupos de creatividades que se verán afectados. Si confirma la eliminación, los grupos de creatividades se modificarán para eliminar la creatividad borrada de la rotación.

<figure><img src="../../.gitbook/assets/image (241).png" alt=""><figcaption><p>Pantalla de confirmación de eliminación que muestra que la creatividad se está utilizando.</p></figcaption></figure>

{% hint style="danger" %}
¡Atención! Si elimina una creatividad, todos los datos relacionados con esa creatividad, incluidas las métricas recopiladas anteriormente, también se eliminarán; esta acción no se puede deshacer.
{% endhint %}

## Monitoreo de creatividades

### Pestaña de métricas

La pestaña de métricas mostrará todas las métricas relacionadas con las creatividades seleccionadas o para toda la cuenta si no hay creatividades seleccionadas. A continuación, encontrará todas las métricas disponibles para sus creatividades.

* [Entregas](ad-server-metrics.md#deliveries-and-delivery-rate)
* [Impresiones y Tasa de Impresión](ad-server-metrics.md#displays-and-display-rate)
* [Visualizaciones](ad-server-metrics.md#views)
* [Visibilidad](ad-server-metrics.md#viewability)
* [Clics y CTR](ad-server-metrics.md#clicks-and-ctr)
* [Tasa de Clic a Carga de Página](ad-server-metrics.md#click-to-page-load-rate)
* [Tiempo hasta la Impresión](ad-server-metrics.md#time-to-display)
* [Tiempo hasta la Visualización](ad-server-metrics.md#time-to-view)
* [Tiempo hasta el Clic](ad-server-metrics.md#time-to-click)
* [Tiempo hasta la Carga de Página](ad-server-metrics.md#time-to-page-load)
* [Cargas de Página](ad-server-metrics.md#page-loads)
* [Tasa de Carga de Página](ad-server-metrics.md#page-load-rate)

### Pestaña de Tiempo Real

La pestaña de tiempo real mostrará eventos en tiempo real relacionados con la creatividad seleccionada.&#x20;

Obtenga más información sobre la [Pestaña de Tiempo Real](../demand-side-platform-dsp/real-time-tab.md).
