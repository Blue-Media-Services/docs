# Almacenamiento de Eventos

En nuestra pestaña de Almacenes de Eventos, puedes crear un almacén que actúe como una base de datos para guardar eventos. Podrás crear un almacén al cual se enviarán tus canalizaciones de eventos. Luego, podrás descargar los eventos como un archivo JSON e importarlos a tu archivo de gestión de datos para organizarlos mejor.

<figure><img src="../../.gitbook/assets/image (296).png" alt="" width="563"><figcaption><p>Event Stores Tab</p></figcaption></figure>

## Creación de un Almacén de Eventos

Para crear un almacén de eventos, haz clic ![Create Event Store](<../../.gitbook/assets/image (977).png>) en y aparecerá una pantalla de creación de eventos.

<figure><img src="../../.gitbook/assets/image (508).png" alt="" width="361"><figcaption><p>Event Store Creation</p></figcaption></figure>

* Nombre - Define un nombre para tu Almacén de Eventos.
* Etiquetas - Crea etiquetas para identificar mejor cada almacén de eventos.
* Retención - Decide por cuánto tiempo conservarás los datos recopilados por este almacén de eventos; una vez vencido el período, los datos serán eliminados.

After configuring your event store, click on ![Save](<../../.gitbook/assets/image (436).png>) button to finish your event creation.

Después de configurar tu almacén de eventos, haz clic en el botón ![Save](/broken/files/Bv5tPEKpmgI5vYwKc6fm) para finalizar la creación.

### Habilitar tu Almacén de Eventos

To enable an event store simply flip the toggle <img src="../../.gitbook/assets/image (510).png" alt="Toggle" data-size="line"> and your event store will be enabled.

Para habilitar un almacén de eventos, simplemente activa el interruptor <img src="/broken/files/FordiXxqA9rxVbNu4piU" alt="Toggle" data-size="line"> y tu almacén quedará habilitado.

<div align="center"><figure><img src="/broken/files/zDkj2tPgCxrISkzJnB7k" alt="" width="148"><figcaption><p>Almacén de Eventos Habilitado</p></figcaption></figure></div>

### Editar tu Almacén de Eventos

Para editar tu almacén de eventos, haz clic en <img src="/broken/files/fjXmu0JbdewJuhhmF3Q6" alt="Edit" data-size="line"> y aparecerá una pantalla de edición. Realiza los cambios necesarios y luego haz clic en ![Save](/broken/files/Bv5tPEKpmgI5vYwKc6fm).

<figure><img src="../../.gitbook/assets/image (513).png" alt="" width="360"><figcaption><p>Edit Event Store Screen</p></figcaption></figure>

### Acciones Masivas

Al seleccionar dos o más almacenes de eventos, se habilitarán las Acciones Masivas, lo que te permitirá realizar acciones en conjunto.

Podrás Archivar, Eliminar, Habilitar y Deshabilitar eventos de forma masiva.

<figure><img src="../../.gitbook/assets/image (266).png" alt=""><figcaption><p>Event Stores' Bulk Actions</p></figcaption></figure>

### Archivar y Desarchivar tu Almacén de Eventos

To archive your event store, click on <img src="../../.gitbook/assets/image (514).png" alt="Archive" data-size="line"> and your event store will be sent to the archived list. In order to unarchive your event store, switch your view to archived events by flipping the toggle <img src="../../.gitbook/assets/image (515).png" alt="Archived Toggle" data-size="line">. You will then be presented with the list of archived events. Click on <img src="../../.gitbook/assets/image (962) (1).png" alt="Unarchive" data-size="line"> to unarchive an event store.

Para archivar tu almacén de eventos, haz clic en <img src="/broken/files/SFOOfUAVFqA2VU2a7V0b" alt="Archive" data-size="line"> y este será enviado a la lista de archivados.\
Para desarchivarlo, cambia tu vista a eventos archivados activando el interruptor <img src="/broken/files/BAWL5ZBRmpnGCEXTPELU" alt="Archived Toggle" data-size="line"> . Luego se mostrará la lista de eventos archivados. Haz clic en <img src="/broken/files/Nr8yowoO1Llbe0Ouejg2" alt="Unarchive" data-size="line"> para desarchivar un almacén de eventos.

### Eliminar tu Almacén de Eventos

To delete an event store, click on <img src="../../.gitbook/assets/image (963) (1).png" alt="Delete" data-size="line"> and a confirmation screen will pop up.

Para eliminar un event store, haz clic en <img src="/broken/files/w3wi5nkUi5gO75A14kjL" alt="Delete" data-size="line"> y aparecerá una pantalla de confirmación.

<figure><img src="../../.gitbook/assets/image (964) (1).png" alt="" width="359"><figcaption><p>Deletion Screen</p></figcaption></figure>

Para confirmar la eliminación, haz clic en ![Delete](<../../.gitbook/assets/image (976).png>).

{% hint style="danger" %}
_¡Atención! Si eliminas un event store, todos los datos relacionados con ese event store serán eliminados._
{% endhint %}

## Flujos de Eventos

Una vez que crees tus almacenes de eventos y _pipes_, todos los eventos activados se mostrarán en la pestaña Flujos de Eventos, estando disponibles para su descarga de acuerdo con tu configuración de retención de datos.\
Estos datos **solo** se mostrarán si existe un _event pipe_ enviando datos a un almacén de eventos.

<figure><img src="/broken/files/jyPiOc6pFYL3toMkXeYQ" alt=""><figcaption><p>Pestaña de Flujo de Eventos</p></figcaption></figure>

### Descarga de tus Flujos de Eventos

You are able to download your event streams by clicking on ![](/broken/files/jGRV9FSkHpSq7QxqUDsW) at the same row as the event stream you want to download. There are two formats of files available:

Puedes descargar tus flujos de eventos haciendo clic en ![](/broken/files/jGRV9FSkHpSq7QxqUDsW) en la misma fila del flujo de eventos que deseas descargar. Existen dos formatos de archivo disponibles:

#### JSON-line

El formato JSON-line ofrece una vista sin procesar y sin filtrar del flujo de eventos, capturando toda la información relevante a medida que ocurren los eventos. Este formato garantiza que no se omita ningún dato, brindándote visibilidad completa de cada transacción para un análisis detallado o integración en flujos de trabajo personalizados.

<figure><img src="../../.gitbook/assets/image (951).png" alt=""><figcaption><p>JSON-line</p></figcaption></figure>

Selecciona este formato y luego haz clic en ![Download](<../../.gitbook/assets/image (978).png>) para descargar tu flujo de eventos.

#### CSV

El formato CSV proporciona una vista personalizable y organizada del flujo de eventos, lo que te permite elegir campos de datos específicos para exportar. Este formato facilita el análisis de los datos en aplicaciones de hojas de cálculo o herramientas de informes, manteniendo la información esencial necesaria para obtener información sobre el rendimiento y la actividad publicitaria.

<figure><img src="../../.gitbook/assets/image (954).png" alt=""><figcaption><p>CSV</p></figcaption></figure>

It is possible to add or remove columns to your CSV file. To add a column click on <img src="/broken/files/sFCayOZc8mpVBM85styC" alt="" data-size="line">, and then fill in the details:

Es posible agregar o eliminar columnas en tu archivo CSV. Para agregar una columna, haz clic en <img src="/broken/files/sFCayOZc8mpVBM85styC" alt="" data-size="line"> , y luego completa los siguientes detalles:

<figure><img src="/broken/files/YVZIhY6aKfcWrPFTbTlb" alt=""><figcaption><p>Agregar Columna</p></figcaption></figure>

* Etiqueta: Indica la etiqueta deseada para la columna
* Leer datos desde: Informa el parámetro del cual deseas leer los datos
* Valor predeterminado: Completa este campo con un valor predeterminado para la columna (opcional).

To remove a column, select it in the list and then click at ![](/broken/files/GOORpYetMOqJfFV66ieD).

Para eliminar una columna, selecciónala en la lista y luego haz clic en ![](/broken/files/GOORpYetMOqJfFV66ieD).

Una vez finalizada tu configuración, haz clic en ![Download](<../../.gitbook/assets/image (978).png>) para descargar tu archivo CSV.

### Acciones en bloque

You can select multiple event streams by checking the <img src="/broken/files/epBkTPeJUBRKG3dxwVLB" alt="Checkbox" data-size="line">, after selecting more than one event, the bulk options will enable, you can download the selected event streams by clicking on <img src="/broken/files/CbGhFAbBPciIly1XtEGS" alt="" data-size="line">, and selecting one of the file formats available.

It's also possible to bulk delete your event streams, click on <img src="/broken/files/8tiAJS772XNzsLuR0R9y" alt="" data-size="line">, then select delete, and confirm the deletion when it is asked.

Puedes seleccionar múltiples flujos de eventos marcando la casilla <img src="/broken/files/epBkTPeJUBRKG3dxwVLB" alt="Checkbox" data-size="line">. Después de seleccionar más de un evento, las opciones en bloque se habilitarán. Puedes descargar los flujos de eventos seleccionados haciendo clic en y seleccionando uno de los formatos de archivo disponibles.

Para realizar descargas masivas de flujos de eventos, puedes seleccionar hasta 100 flujos de eventos individuales o seleccionar todos los flujos de eventos.

También es posible eliminar flujos de eventos en bloque. Haz clic en <img src="/broken/files/8tiAJS772XNzsLuR0R9y" alt="" data-size="line">, luego selecciona eliminar, y confirma la eliminación cuando se te solicite.

### Eliminación de Flujos de Eventos

Para eliminar un evento, haz clic en ![](/broken/files/b13HqBPcE8eBnNEDxKRe) y se requerirá una confirmación.

<figure><img src="/broken/files/PiW98WWh3s3TUBaY7Mq7" alt="" width="359"><figcaption><p>Eliminación de Evento</p></figcaption></figure>

Después de hacer clic en ![Delete](<../../.gitbook/assets/image (976).png>), tus datos de eventos se eliminarán de forma permanente.

{% hint style="danger" %}
_¡Atención! Ten cuidado al eliminar flujos de eventos, esta acción no se puede deshacer, lo que significa que tus datos se eliminarán permanentemente._
{% endhint %}

## **Pestaña de Métricas**

Selecciona un almacén de eventos para visualizar las métricas generadas por los _event pipes_. Ten en cuenta que debes seleccionar un almacén de eventos al crear un _event pipe_. Si envías tus eventos únicamente a un _webhook_, el almacén de eventos no se poblará. Estas son todas las métricas disponibles para los almacenes de eventos:

* [Stream Bytes](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-bytes)
* [Stream Count](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-count)
* [Stream Upload Bytes](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-upload-bytes)
* [Stream Upload Count](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-upload-count)
* [Stream Download Bytes](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-download-bytes)
* [Stream Download Count](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-download-count)
* [Stream Delete Bytes](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-delete-bytes)
* [Stream Delete Count](../../../es/product-documentation/monitoring/monitoring-metrics.md#stream-delete-count)
