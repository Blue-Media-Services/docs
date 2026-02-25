# Pipelines de Eventos

Nuestros Pipelines de Eventos se utilizan para recopilar datos de todos los productos de nuestra plataforma. Puede utilizar esta función para realizar un seguimiento de todo lo que puede provocar un evento en BMS, desde campañas hasta la creación de organizaciones, lo que le permite organizar los datos proporcionados como desee.

Todas las tuberías de eventos creadas se enviarán a un almacén de eventos, o bien puede utilizar un webhook para enviar estos datos directamente a su herramienta de gestión de datos. Proporcionamos plantillas para cada evento que podemos rastrear, de modo que pueda elegir cuáles desea recopilar.

{% hint style="info" %}
Tenemos una solución que puede ayudarte a comprender cómo funciona un webhook. Consulta este artículo [aquí](../../integraciones-de-terceros/webhook-tool-zapier.md).
{% endhint %}

## Creación de un Pipeline de Eventos

Para crear un almacén de eventos, haga clic en <img src="../../.gitbook/assets/image (190).png" alt="Create Event Pipe" data-size="line"> , y aparecerá una pantalla para crear un canal de eventos.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 073841.png" alt=""><figcaption><p>Creación de Pipeline de Eventos</p></figcaption></figure>

* Nombre: Establezca un nombre para su almacén de eventos.
* Etiquetas: Cree etiquetas para identificar mejor cada canal de eventos.

### Filtros

Para empezar a configurar tu canal de eventos, elige la plantilla que prefieras en nuestra pestaña Filtros según tus necesidades.

* Plantilla de evento de muestra - In este menú desplegable, se le proporcionarán todas las plantillas relacionadas con los eventos que podemos rastrear.

En este ejemplo, crearemos un canal de eventos para ADS - Delivered. Este evento realiza un seguimiento de todos los anuncios que se están ejecutando actualmente en una campaña y que están generando impresiones. Una vez creado este canal de eventos, todos los datos se enviarán a un almacén de eventos o a un webhook.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 074141.png" alt=""><figcaption><p>ADS - Anuncio entregado Canal de eventos</p></figcaption></figure>

Una vez seleccionada la plantilla, puede comprobar qué datos se recopilarán al crear el pipeline de eventos correspondiente.

Para recopilar los datos, **debemos** insertar un filtro haciendo clic en ![Add Filter](<../../.gitbook/assets/image (279).png>).

<figure><img src="../../.gitbook/assets/image (78).png" alt="" width="515"><figcaption><p>Agregar Filtros</p></figcaption></figure>

* Ruta - Etiqueta específica en la que se puede identificar el evento. Ejemplo: id, tipo, fuente, data.accountId.
* Operador - Regla que se utilizará en este filtro.
* Valor - El valor específico que debe contener la etiqueta.

En este caso, recopilaremos datos de eventos relacionados con la entrega de anuncios, por lo que la configuración sería la siguiente:

<figure><img src="../../.gitbook/assets/image (195).png" alt="" width="524"><figcaption><p>Configuración del filtro de eventos</p></figcaption></figure>

Especificamos la **ruta** utilizando la etiqueta "Tipo", seleccionamos la **opción** "Contiene" en el operador y añadimos el **valor** "Anuncio entregado". Tenga en cuenta que estos campos distinguen entre mayúsculas y minúsculas, por lo que los campos rellenados deben coincidir con la plantilla.

Una vez que haya completado todos los campos con la información correspondiente basada en su canal de eventos, el filtro de prueba debe tener una marca que confirme que funciona correctamente <img src="../../.gitbook/assets/image (196).png" alt="Test Filters Checked" data-size="line">. Si no funciona correctamente debido a información faltante o un error tipográfico, se mostrará una señal de advertencia <img src="../../.gitbook/assets/image (284).png" alt="Test Filters Warning" data-size="line">.

<figure><img src="../../.gitbook/assets/image (197).png" alt="" width="518"><figcaption><p>Advertencia del filtro de prueba</p></figcaption></figure>

En este caso, nuestro filtro falló debido a la verificación en nuestro campo Valor. Estos campos distinguen entre mayúsculas y minúsculas y **deben** coincidir con la información correspondiente.

Una vez que hayas añadido tus filtros, haz clic en <img src="../../.gitbook/assets/image (92) (2).png" alt="" data-size="line"> para guardar tu evento.

### Pestaña Objetivos

Aquí decidirás dónde enviar los datos: si se enviarán a uno o varios almacenes de eventos, a un webhook o a una hoja de cálculo de Google.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 074833.png" alt=""><figcaption><p>Pestaña Objetivos de Pipeline de Eventos</p></figcaption></figure>

Para configurar un objetivo, haga clic en ![Add Target](<../../.gitbook/assets/Captura de tela 2024-11-01 083709.png>) y rellene los datos según la opción de destino elegida:

#### Enviar a la Almacén de Eventos

Debe crear un almacén de eventos antes de utilizarlo como destino para sus canalizaciones de eventos. Más información sobre [Pipelines de Eventos](event-pipes.md#event-store).

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Enviar al Target de Almacén de Eventos</p></figcaption></figure>

Si decides enviar tus datos a un almacén de eventos, simplemente nombra tu destino y elige el almacén de eventos que ya has creado.

* Nombra tu objetivo.
* Seleccione "Enviar al almacén de eventos".
* Seleccione el almacén de eventos que desea utilizar.

Una vez que todo esté configurado, haga clic en <img src="../../.gitbook/assets/image (203).png" alt="Save" data-size="line"> y aparecerá tu canal de eventos.

#### Llamar a Webhook

Es posible enviar sus datos a un webhook proporcionado por su herramienta de gestión de datos. Seleccione esta opción para utilizar la herramienta de gestión de datos que prefiera y, a continuación, rellene los datos.

<figure><img src="../../.gitbook/assets/image (93) (1).png" alt=""><figcaption><p>Objetivo de Llamada a Webhook</p></figcaption></figure>

* Nombra tu objetivo.
* Selecciona "Llamar a Webhook".
* Introduzca la URL del webhook de su herramienta de gestión de datos.

Una vez que haya configurado la URL de su webhook, utilice nuestra pestaña Probar webhook para confirmar la usabilidad de su herramienta webhook. Seleccione una de las plantillas de eventos de muestra y haga clic en ![Test Webhook](<../../.gitbook/assets/image (94) (1).png>).

Si la prueba de tu webhook es satisfactoria, tu icono se mostrará como ![Test Webhook Successful](<../../.gitbook/assets/image (8) (2).png>) y se completarán las pestañas para su prueba.

* Carga útil - Información que se enviará a tu webhook.
* Resultado - Estado devuelto y latencia.
* Solicitud - Solicitud utilizada por BMS para enviarle la información relativa a esta prueba.
* Respuesta - Se ha recibido la respuesta de su webhook.

Después de terminar toda la configuración y las pruebas, haga clic en <img src="../../.gitbook/assets/image (92) (2).png" alt="" data-size="line"> para salvar a tu objetivo.

#### Google Sheets

También puede enviar sus datos a Google Sheets, seleccione esta opción y rellene los datos.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Objetivo de Google Sheet</p></figcaption></figure>

* Nombra tu objetivo.
* Seleccionar "Google Sheets".
* Conéctate con tu cuenta de Google y podrás acceder a la sheet.

Una vez que todo esté configurado, haga clic en <img src="../../.gitbook/assets/image (203).png" alt="Save" data-size="line"> y aparecerá tu canal de eventos.

### Habilitar su Canal de Eventos

Para habilitar un canal de eventos, simplemente active el interruptor <img src="../../.gitbook/assets/image (510).png" alt="Toggle" data-size="line"> y tu tienda de eventos quedará habilitada.

<figure><img src="../../.gitbook/assets/image (75).png" alt=""><figcaption><p>Pipeline de Eventos Habilitado</p></figcaption></figure>

### Edición de su Canal de Eventos

Para editar tu tienda de eventos, haz clic en <img src="../../.gitbook/assets/image (512).png" alt="Edit" data-size="line"> y aparecerá una pantalla de edición, realice los cambios necesarios y luego haga clic en <img src="../../.gitbook/assets/image (509).png" alt="Save" data-size="line">.

<figure><img src="../../.gitbook/assets/image (77).png" alt="" width="527"><figcaption><p>Pantalla de Edición del Pipeline de Eventos</p></figcaption></figure>

### Acciones Masivas

Al seleccionar dos o más tuberías de eventos, se habilitarán las acciones masivas, lo que le permitirá realizar acciones de forma masiva.

Podrás archivar y eliminar eventos de forma masiva.

<figure><img src="../../.gitbook/assets/image (76).png" alt=""><figcaption><p>Acciones Masivas del Pipeline de Eventos</p></figcaption></figure>

### Archivar y Desarchivar su Canal de Eventos

Para archivar tu canal de eventos, haz clic en <img src="../../.gitbook/assets/image (514).png" alt="Archive" data-size="line"> y se enviará a la lista archivada. Para desarchivar tu canal de eventos, cambia la vista a eventos archivados activando el botón <img src="../../.gitbook/assets/image (515).png" alt="Archived Toggle" data-size="line">. A continuación, se le mostrará la lista de eventos archivados. Haga clic en <img src="../../.gitbook/assets/image (876).png" alt="Unarchive" data-size="line"> para desarchivar un canal de eventos.

### Eliminar tu Canal de Eventos

Para eliminar un evento, haga clic en ![](<../../.gitbook/assets/image (975).png>) y se requerirá una confirmación.

<figure><img src="../../.gitbook/assets/image (93).png" alt=""><figcaption><p>Eliminación del Pipeline de Eventos</p></figcaption></figure>

Después de hacer clic en <img src="../../.gitbook/assets/image (977).png" alt="Delete" data-size="line">, tu canal de eventos será eliminado.

{% hint style="warning" %}
_Recomendamos a los usuarios que archiven en lugar de eliminar; solo elimine si está seguro, ya que la acción no se puede deshacer._
{% endhint %}

## Pestaña Métricas

Seleccione una canalización de eventos para acceder a sus métricas. Si selecciona más de una, se mostrará una comparación entre las seleccionadas. Las métricas se rellenan una vez que ha creado las canalizaciones de eventos y estas están habilitadas y recopilando datos.

Estas son todas las métricas para los conductos de eventos:

* [Recuento de Eventos Coincidentes](monitoring-metrics.md#matched-events-count)
* [Recuento de Llamadas de Ejecución del Objetivo](monitoring-metrics.md#target-execution-call-count)
* [Tasa de fallos de Ejecución del Objetivo](monitoring-metrics.md#target-execution-failure-rate)
