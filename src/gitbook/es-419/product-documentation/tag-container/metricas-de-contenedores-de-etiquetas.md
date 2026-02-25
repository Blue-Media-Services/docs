# Métricas de Contenedores de Etiquetas

Seleccione un contenedor de etiquetas de la lista para mostrar las métricas relacionadas con él en la pestaña de métricas. Si no selecciona ninguno, se mostrarán las métricas de toda la cuenta para todos sus contenedores de etiquetas, y si selecciona más de uno, se mostrará una comparación entre los seleccionados. Además, al revisar las métricas, siempre puede utilizar el <img src="../../.gitbook/assets/image (462).png" alt="" data-size="line"> para acceder a nuestros artículos sobre una métrica específica.

{% hint style="info" %}
Puede obtener más información sobre cómo se gestionan las métricas visitando la página [Métricas](../metricas.md).
{% endhint %}

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-10 082108.png" alt=""><figcaption><p>Contenedores de etiquetas - Pestaña Métricas</p></figcaption></figure>

### Tasa de Fallos

Esta métrica indica, en porcentaje, la frecuencia con la que se solicitó un contenedor de etiquetas, pero la solicitud falló dentro del plazo definido.

<div data-full-width="false"><figure><img src="../../.gitbook/assets/Failure Rate.png" alt=""><figcaption><p>Métrica de Tasa de fallos</p></figcaption></figure></div>

_**Ejemplo:** En esta imagen, el marco de tiempo definido fue de 1 semana, dividido en períodos diarios. Dado que esta métrica muestra la tasa de fallos, lo ideal es que los resultados sean lo más bajos posible. Notará que, en este caso, la tasa de fallos fue del 0%, lo que significa que ninguna solicitud falló durante este período._

### Recuento de Solicitudes

Esta métrica representa el número de veces que se solicitaron los contenedores de etiquetas seleccionados dentro del marco de tiempo definido.

<div data-full-width="true"><figure><img src="../../.gitbook/assets/request count.png" alt=""><figcaption><p>Métrica de Recuento de Solicitudes</p></figcaption></figure></div>

_**Ejemplo:** Se contabiliza una solicitud cada vez que el contenedor de etiquetas se renderiza durante la carga de su sitio web, de acuerdo con su instalación. En esta imagen, puede observar que el marco de tiempo definido fue de 1 semana, dividido en períodos diarios. Cada línea representa un contenedor de etiquetas diferente seleccionado de la lista. Por ejemplo, la línea azul muestra algo más de 1,000 solicitudes diarias durante los primeros 4 días, luego disminuyó a casi 400 solicitudes el 28 de septiembre y fluctuó entre 400 y 700 solicitudes durante el resto de la semana._
