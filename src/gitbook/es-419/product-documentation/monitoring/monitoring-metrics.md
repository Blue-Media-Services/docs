# Métricas de Monitoreo

Estas son todas las métricas disponibles en la función de supervisión para analizar los datos proporcionados por los eventos configurados. La pestaña Métricas de almacenes de eventos mostrará los eventos relacionados con todas las tuberías de eventos que se han producido y estarán disponibles para su descarga. La pestaña Tuberías de eventos mostrará las métricas relacionadas con todas las tuberías creadas, lo que le permitirá saber si las tuberías funcionan correctamente.&#x20;

{% hint style="info" %}
Para obtener más información sobre cómo se gestionan las métricas, visite la página [Métricas](../metricas.md).
{% endhint %}

### Bytes de Flujo

Se rellena con los flujos de eventos disponibles para su descarga. Según el tamaño de cada flujo de eventos, esta métrica presentará la suma de todos los bytes de sus flujos de eventos.

<figure><img src="../../.gitbook/assets/Stream Bytes.png" alt=""><figcaption><p>Bytes de Flujo</p></figcaption></figure>

_**Ejemplo:** Después de haber poblado un almacén de eventos (event store), este presentará flujos de eventos (event streams) relacionados con los conductos (pipes) seleccionados. Entonces podrá comprobar el tamaño y la fecha de cada flujo por separado. El gráfico se poblará a medida que aumente el tamaño del flujo. En este gráfico es posible ver que alcanzó un tamaño de casi 2 MB en una semana._

### Recuento de Flujos

Esta métrica presenta el recuento de cada flujo de eventos presente en su almacén de eventos; si el almacén de eventos tiene muchos conductos relacionados, el recuento será elevado.

<figure><img src="../../.gitbook/assets/Stream Count.png" alt=""><figcaption><p>Recuento de Flujos</p></figcaption></figure>

_**Ejemplo:** Al crear conductos de eventos (event pipes), debe seleccionar un almacén de eventos o un webhook para enviar los datos. Una vez que selecciona un almacén de eventos, cada conducto que cree hacia ese mismo almacén generará un flujo de eventos al recibir datos. Es importante tener en cuenta que, si tiene demasiados conductos de eventos hacia el mismo almacén, es aconsejable separarlos para organizar mejor sus flujos de eventos. En este gráfico, puede ver que el recuento de flujos alcanzó un pico de casi 200 flujos._

### Bytes de Subida de Flujo

Presenta la cantidad total de bytes subidos a la pestaña de flujos de eventos, dejando los flujos disponibles para su descarga.

<figure><img src="../../.gitbook/assets/Stream Upload Bytes.png" alt=""><figcaption><p>Bytes de Subida de Flujo</p></figcaption></figure>

_**Ejemplo:** Cada flujo de eventos se sube a su almacén de eventos seleccionado después de unos minutos, quedando disponible para su descarga como un archivo .JSON. La métrica presentará la suma de todos los bytes de los flujos de eventos subidos a su almacén de eventos. En este gráfico, podemos ver que en fechas específicas los datos se redujeron significativamente debido a la fecha de expiración de cada flujo de eventos o a su eliminación._

### Recuento de Subida de Flujos

Esta métrica presenta el recuento total de subidas relacionadas con los datos recolectados y presentados para descarga de cada flujo de eventos; una vez que estos expiren o sean eliminados, el recuento disminuirá.

<figure><img src="../../.gitbook/assets/stream upload count.png" alt=""><figcaption><p>Recuento de Subida de Flujos</p></figcaption></figure>

_**Ejemplo:** En este gráfico, es posible ver que en algunas fechas el recuento llegó casi a cero debido a que no había conductos de eventos activos o a causa de una limpieza. Es importante verificar su recuento de subidas, ya que podría afectar la forma en que organiza sus flujos de eventos. Tener demasiados flujos de eventos que organizar puede resultar confuso, por lo que se debe realizar una limpieza u optimización de vez en cuando._

### Bytes de Descarga de Flujo

Esta métrica representa la suma de todos los bytes descargados de sus flujos de eventos y se poblará únicamente cuando el flujo de eventos haya sido descargado.

<figure><img src="../../.gitbook/assets/Stream Download Bytes.png" alt=""><figcaption><p>Bytes de Descarga de Flujo</p></figcaption></figure>

_**Ejemplo:** Una vez que comience a descargar los datos de sus flujos de eventos, se le informará del número total de bytes descargados cada día. Esto le ayuda a realizar un seguimiento de cuánta información se ha descargado. Si el volumen de datos es alto, indica que se capturaron muchos eventos del flujo de eventos. En este gráfico, puede ver que solo se descargaron 2 KB de datos._

### Recuento de Descargas de Flujo

Esta métrica representa los flujos de eventos descargados y se poblará cada vez que usted descargue un flujo de eventos.

<figure><img src="../../.gitbook/assets/Stream Download Count.png" alt=""><figcaption><p>Recuento de Descargas de Flujo</p></figcaption></figure>

_**Ejemplo:** Si se organiza para descargar los datos recolectados de los conductos de eventos cada semana o cada dos semanas, la métrica le informará para que no pierda el hilo de su cronograma establecido. En este gráfico, puede ver que los flujos de eventos se descargaron solo después de una semana._

### Bytes de Eliminación de Flujo

Esta métrica se puebla cada vez que se elimina un flujo de eventos, mostrándole la suma de todos los bytes eliminados, ya sea manualmente o por la fecha de retención establecida al crear el almacén de eventos.

<figure><img src="../../.gitbook/assets/Stream Delete Bytes.png" alt=""><figcaption><p>Bytes de Eliminación de Flujo</p></figcaption></figure>

_**Ejemplo:** Una vez que comience a recopilar datos para su almacén de eventos, establecerá una fecha de retención para los mismos. Cada vez que los datos alcancen esa fecha, su flujo de eventos se eliminará; también puede eliminarlos manualmente. En este gráfico, puede ver que, en un momento dado, se eliminaron casi todos los flujos de eventos._

### Recuento de Eliminación de Flujos

Esta métrica representa el recuento total de flujos de eventos eliminados; se pobla ya sea por eliminación por retención o por eliminación manual.

<figure><img src="../../.gitbook/assets/Stream Delete Count.png" alt=""><figcaption><p>Recuento de Eliminación de Flujos</p></figcaption></figure>

_**Ejemplo:** En este gráfico, puede ver que el recuento de eliminaciones sigue un patrón, pero en algunas fechas se eliminó una cantidad menor. Esto podría deberse a un cambio en la fecha de retención o a que se habilitaron menos flujos de eventos. Eliminar datos puede ayudarle a mantenerlos más organizados._

### Recuento de Eventos Coincidentes

Esta métrica se puebla cada vez que un evento coincide con los criterios de su conducto (pipe) de eventos; una vez que cumple con su configuración, comienza a recolectar datos.

<figure><img src="../../.gitbook/assets/Matched Events Count.png" alt=""><figcaption><p>Recuento de Eventos Coincidentes</p></figcaption></figure>

_**Ejemplo:** Cada vez que un evento cumple con los criterios establecidos durante la creación del conducto de eventos (event pipe), esta métrica se actualizará. Es importante monitorear esta métrica, ya que indica si los criterios se están cumpliendo correctamente; de lo contrario, no habrá datos para recolectar. En este gráfico, puede ver que en un momento dado alcanzó un pico de casi 250,000 eventos. La métrica variará en función del número de campañas que se estén ejecutando en ese momento._

### Recuento de Llamadas de Ejecución de Destino

Esta métrica se puebla después de que los eventos coincidentes tienen éxito; cada evento coincidente se enviará a una llamada de ejecución de destino según los criterios establecidos. Esta métrica casi siempre seguirá los mismos parámetros que el recuento de eventos coincidentes.

<figure><img src="../../.gitbook/assets/Target Execution Call Count.png" alt=""><figcaption><p>Recuento de Llamadas de Ejecución de Destino</p></figcaption></figure>

_**Ejemplo:** Después de que un evento coincide con los criterios, nuestro sistema ejecutará el conducto de eventos (event pipe) establecido, recopilará los datos según los parámetros y luego los enviará a un almacén de eventos o webhook, según lo configurado. En este gráfico, puede ver el recuento de eventos coincidentes._

### Tasa de Fallo de Ejecución de Destino

Esta métrica se puebla con los fallos de una ejecución de llamada; si hay algún error, inestabilidad en la plataforma o en la configuración del conducto de eventos, nuestro sistema poblará la métrica de tasa de fallos.

<figure><img src="../../.gitbook/assets/Target Execution Failure Rate.png" alt=""><figcaption><p>Tasa de Fallo de Ejecución de Destino</p></figcaption></figure>

_**Ejemplo:** Si falla la ejecución de una llamada, compruebe la configuración de su canal de eventos o si la plataforma está experimentando inestabilidad, ya que esto puede provocar que falle la ejecución de la llamada. En este gráfico, puede ver que, durante un mes, hubo una tasa de fallos del 1 % en un día, seguida de ningún fallo posterior._
