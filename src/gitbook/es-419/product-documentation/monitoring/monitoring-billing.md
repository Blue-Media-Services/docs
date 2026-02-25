# Facturación de Monitoreo

En la pestaña de monitoreo, se presentarán todas las facturas relacionadas con el monitoreo, que se dividen en 4 subsecciones.

<figure><img src="../../.gitbook/assets/image (312).png" alt=""><figcaption><p>Subsecciones de supervisión</p></figcaption></figure>

{% hint style="info" %}
En BMS, se prioriza la transparencia mostrando todos los detalles de su factura. Visite nuestro [Facturación](../billing.md) para comprender cómo están estructurados los proyectos de ley.
{% endhint %}

### Gestión de Pipelines de Eventos

Cada acción realizada en un canal de eventos generará una solicitud. Por ejemplo, crear un canal de eventos, enumerar sus canales de eventos y realizar cambios en un canal de eventos generará una solicitud. Además, cada canal de eventos creará registros de eventos por hora, que se cobrarán en función de un período de 720 horas.

<figure><img src="../../.gitbook/assets/image (671).png" alt=""><figcaption><p>Gestión detallada de pipeline de eventos</p></figcaption></figure>

_**Ejemplo:** En esta factura, solo se ha cobrado el conducto de eventos (event pipe) configurado. Al observar el número de horas, se puede ver que el conducto ha estado activo durante un mes y algunos días, lo que resulta en una factura total de $0.79. No se produjeron otros cargos ya que ninguna solicitud superó las primeras 1,000 solicitudes gratuitas._

### Gestión del Almacén de Eventos

En la página del Almacén de Eventos, todas las acciones contarán como una solicitud. Si accede a la página, crea un almacén de eventos, consulta sus flujos de eventos disponibles o descarga un flujo de eventos, cada una de estas acciones contará como una solicitud. Sin embargo, la descarga de un flujo de eventos también generará cargos, al igual que el almacenamiento de los mismos. Estos cargos se basarán en el tamaño del flujo de eventos y la duración de su almacenamiento en BMS.

<figure><img src="../../.gitbook/assets/image (309).png" alt=""><figcaption><p>Gestión detallada del Almacén de Eventos</p></figcaption></figure>

_**Ejemplo:** En esta factura, es posible ver que la mayoría de las solicitudes no fueron cobradas al no alcanzar las 1,000 solicitudes gratuitas. Sin embargo, las solicitudes del almacén de eventos generaron una factura de $1.95 debido a la gran cantidad de flujos de eventos generados dentro de ese almacén. Tener un almacén de eventos configurado también generó cargos porque los flujos de eventos se crean cada hora, resultando en una factura de $0.47. Además, el almacenamiento de estos flujos generados en el servidor BMS (si no se utiliza la función de webhook) generó una factura de $0.04, lo que eleva la factura total a $2.46._

### Monitoreo de Métricas

Todas las métricas en cualquier plataforma generan cargos y son cruciales para analizar el rendimiento y tomar decisiones estratégicas basadas en los datos recopilados. BMS centraliza los cargos de cada métrica de la plataforma bajo la pestaña Monitoring, que es responsable de recibir todos los eventos dentro de la plataforma.

Las métricas se cobran por cada punto registrado y por los bytes procesados por los servidores de BMS para generar dichas métricas.

<figure><img src="../../.gitbook/assets/image (587).png" alt=""><figcaption><p>Monitorización métrica detallada</p></figcaption></figure>

_**Ejemplo:** En esta factura, se observa que se acumularon casi 17 millones de puntos de métrica en un mes. Este total se genera sumando todas las métricas de la cuenta del usuario, lo que resulta en un coste de $83.47. Además, la cantidad de datos escaneados para generar estas métricas fue de casi 119 mil GB, lo que supuso un cargo de $2.37, para una factura total de $85.84._

### Monitoreo en Tiempo Real

Algunos productos disponen de una pestaña de tiempo real que muestra los eventos de su campaña a medida que ocurren. Por ejemplo, cuando se muestra un anuncio, se visualizará la ubicación del usuario según el _ad exchange_ utilizado, junto con información adicional. Cada vez que se acceda a la pestaña de tiempo real, se generarán costes.

<figure><img src="../../.gitbook/assets/image (588).png" alt=""><figcaption><p>Monitoreo en Tiempo Real</p></figcaption></figure>

_**Ejemplo:** En este caso, las solicitudes de eventos recientes en tiempo real fueron relativamente bajas, pero superaron la marca de 100 000 eventos gratuitos, lo que dio lugar a un cargo de 0,14$._
