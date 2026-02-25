# Almacenamiento de Eventos

En nuestra pestaña de Almacenes de Eventos, puedes crear un almacén que actúe como una base de datos para guardar eventos. Podrás crear un almacén al cual se enviarán tus canalizaciones de eventos. Luego, podrás descargar los eventos como un archivo JSON e importarlos a tu archivo de gestión de datos para organizarlos mejor.

<figure><img src="../../.gitbook/assets/image (296).png" alt="" width="563"><figcaption><p>Pestaña Tiendas de eventos</p></figcaption></figure>

## Creación de un Almacén de Eventos

Para crear un almacén de eventos, haz clic ![Create Event Store](<../../.gitbook/assets/image (90) (1).png>) en y aparecerá una pantalla de creación de eventos.

<figure><img src="../../.gitbook/assets/image (508).png" alt="" width="361"><figcaption><p>Creación de tienda de eventos</p></figcaption></figure>

* Nombre - Define un nombre para tu Almacén de Eventos.
* Etiquetas - Crea etiquetas para identificar mejor cada almacén de eventos.
* Retención - Decide por cuánto tiempo conservarás los datos recopilados por este almacén de eventos; una vez vencido el período, los datos serán eliminados.

Después de configurar tu almacén de eventos, haz clic en el botón ![Save](<../../.gitbook/assets/image (97).png>) para finalizar la creación.

### Habilitar tu Almacén de Eventos

Para habilitar un almacén de eventos, simplemente activa el interruptor <img src="../../.gitbook/assets/image (79).png" alt="Toggle" data-size="line"> y tu almacén quedará habilitado.

<div align="center"><figure><img src="../../.gitbook/assets/image (80).png" alt="" width="148"><figcaption><p>Almacén de Eventos Habilitado</p></figcaption></figure></div>

### Editar tu Almacén de Eventos

Para editar tu almacén de eventos, haz clic en <img src="../../.gitbook/assets/image (81).png" alt="Edit" data-size="line"> y aparecerá una pantalla de edición. Realiza los cambios necesarios y luego haz clic en ![Save](<../../.gitbook/assets/image (97).png>).

<figure><img src="../../.gitbook/assets/image (513).png" alt="" width="360"><figcaption><p>Editar pantalla del almacén de eventos</p></figcaption></figure>

### Acciones Masivas

Al seleccionar dos o más almacenes de eventos, se habilitarán las Acciones Masivas, lo que te permitirá realizar acciones en conjunto.

Podrás Archivar, Eliminar, Habilitar y Deshabilitar eventos de forma masiva.

<figure><img src="../../.gitbook/assets/image (266).png" alt=""><figcaption><p>Acciones masivas de las tiendas de eventos</p></figcaption></figure>

### Archivar y Desarchivar tu Almacén de Eventos

Para archivar tu almacén de eventos, haz clic en <img src="../../.gitbook/assets/image (82).png" alt="Archive" data-size="line"> y este será enviado a la lista de archivados.\
Para desarchivarlo, cambia tu vista a eventos archivados activando el interruptor <img src="../../.gitbook/assets/image (83).png" alt="Archived Toggle" data-size="line"> . Luego se mostrará la lista de eventos archivados. Haz clic en <img src="../../.gitbook/assets/image (91).png" alt="Unarchive" data-size="line"> para desarchivar un almacén de eventos.

### Eliminar tu Almacén de Eventos

Para eliminar un event store, haz clic en <img src="../../.gitbook/assets/image (92).png" alt="Delete" data-size="line"> y aparecerá una pantalla de confirmación.

<figure><img src="../../.gitbook/assets/image (878).png" alt="" width="359"><figcaption><p>Pantalla de eliminación</p></figcaption></figure>

Para confirmar la eliminación, haz clic en ![Delete](<../../.gitbook/assets/image (89) (1).png>).

{% hint style="danger" %}
_¡Atención! Si eliminas un event store, todos los datos relacionados con ese event store serán eliminados._
{% endhint %}

## Flujos de Eventos

Una vez que crees tus almacenes de eventos y _pipes_, todos los eventos activados se mostrarán en la pestaña Flujos de Eventos, estando disponibles para su descarga de acuerdo con tu configuración de retención de datos.\
Estos datos **solo** se mostrarán si existe un _event pipe_ enviando datos a un almacén de eventos.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-28 072309.png" alt=""><figcaption><p>Pestaña de Flujo de Eventos</p></figcaption></figure>

### Descarga de tus Flujos de Eventos

Puedes descargar tus flujos de eventos haciendo clic en ![](<../../.gitbook/assets/image (85).png>) en la misma fila del flujo de eventos que deseas descargar. Existen dos formatos de archivo disponibles:

#### JSON-line

El formato JSON-line ofrece una vista sin procesar y sin filtrar del flujo de eventos, capturando toda la información relevante a medida que ocurren los eventos. Este formato garantiza que no se omita ningún dato, brindándote visibilidad completa de cada transacción para un análisis detallado o integración en flujos de trabajo personalizados.

<figure><img src="../../.gitbook/assets/image (865).png" alt=""><figcaption><p>JSON-line</p></figcaption></figure>

Selecciona este formato y luego haz clic en ![Download](<../../.gitbook/assets/image (91) (1).png>) para descargar tu flujo de eventos.

#### CSV

El formato CSV proporciona una vista personalizable y organizada del flujo de eventos, lo que te permite elegir campos de datos específicos para exportar. Este formato facilita el análisis de los datos en aplicaciones de hojas de cálculo o herramientas de informes, manteniendo la información esencial necesaria para obtener información sobre el rendimiento y la actividad publicitaria.

<figure><img src="../../.gitbook/assets/image (868).png" alt=""><figcaption><p>CSV</p></figcaption></figure>

Es posible agregar o eliminar columnas en tu archivo CSV. Para agregar una columna, haz clic en <img src="../../.gitbook/assets/image (87).png" alt="" data-size="line"> , y luego completa los siguientes detalles:

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption><p>Agregar Columna</p></figcaption></figure>

* Etiqueta: Indica la etiqueta deseada para la columna
* Leer datos desde: Informa el parámetro del cual deseas leer los datos
* Valor predeterminado: Completa este campo con un valor predeterminado para la columna (opcional).

Para eliminar una columna, selecciónala en la lista y luego haz clic en ![](<../../.gitbook/assets/image (88).png>).

Una vez finalizada tu configuración, haz clic en ![Download](<../../.gitbook/assets/image (91) (1).png>) para descargar tu archivo CSV.

### Acciones en bloque

Puedes seleccionar múltiples flujos de eventos marcando la casilla <img src="../../.gitbook/assets/image (94).png" alt="Checkbox" data-size="line">. Después de seleccionar más de un evento, las opciones en bloque se habilitarán. Puedes descargar los flujos de eventos seleccionados haciendo clic en <img src="../../.gitbook/assets/image (89).png" alt="" data-size="line">, y seleccionando uno de los formatos de archivo disponibles.

Para realizar descargas masivas de flujos de eventos, puedes seleccionar hasta 100 flujos de eventos individuales o seleccionar todos los flujos de eventos.

También es posible eliminar flujos de eventos en bloque. Haz clic en <img src="../../.gitbook/assets/image (90).png" alt="" data-size="line">, luego selecciona eliminar, y confirma la eliminación cuando se te solicite.

### Eliminación de Flujos de Eventos

Para eliminar un evento, haz clic en ![](<../../.gitbook/assets/image (95).png>) y se requerirá una confirmación.

<figure><img src="../../.gitbook/assets/image (96).png" alt="" width="359"><figcaption><p>Eliminación de Evento</p></figcaption></figure>

Después de hacer clic en ![Delete](<../../.gitbook/assets/image (89) (1).png>), tus datos de eventos se eliminarán de forma permanente.

{% hint style="danger" %}
_¡Atención! Ten cuidado al eliminar flujos de eventos, esta acción no se puede deshacer, lo que significa que tus datos se eliminarán permanentemente._
{% endhint %}

## **Pestaña de Métricas**

Selecciona un almacén de eventos para visualizar las métricas generadas por los _event pipes_. Ten en cuenta que debes seleccionar un almacén de eventos al crear un _event pipe_. Si envías tus eventos únicamente a un _webhook_, el almacén de eventos no se poblará. Estas son todas las métricas disponibles para los almacenes de eventos:

* [Bytes de Transmisión](monitoring-metrics.md#stream-bytes)
* [Recuento de Transmisiones](monitoring-metrics.md#stream-count)
* [Bytes de carga de Transmisión](monitoring-metrics.md#stream-upload-bytes)
* [Recuento de carga de Transmisión](monitoring-metrics.md#stream-upload-count)
* [Bytes de descarga de Transmisión](monitoring-metrics.md#stream-download-bytes)
* [Recuento de descarga de Transmisión](monitoring-metrics.md#stream-download-count)
* [Bytes de eliminación de Transmisión](monitoring-metrics.md#stream-delete-bytes)
* [Recuento de eliminación de Transmisión](monitoring-metrics.md#stream-delete-count)
