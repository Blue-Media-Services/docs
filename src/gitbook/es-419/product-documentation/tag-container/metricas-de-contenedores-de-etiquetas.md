# Métricas de Contenedores de Etiquetas

Select a Tag Container from the list to display the metrics related to it on the metrics tab. Selecting none will show you account-wide metrics for all your Tag Containers, and selecting more than one will display a comparison between the selected ones. Additionally, when reviewing metrics, you can always use the <img src="../../../es-419/.gitbook/assets/image (462).png" alt="" data-size="line"> to access our articles about a specific metric.

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../../../es-419/product-documentation/metricas.md).
{% endhint %}

<figure><img src="../../../es-419/.gitbook/assets/Captura de tela 2024-12-10 082108.png" alt=""><figcaption><p>Tag Containers - Metrics Tab</p></figcaption></figure>

### Failure Rate

This metric indicates, as a percentage, the frequency at which a tag container was requested but the request failed within the defined time frame.

<div data-full-width="false"><figure><img src="../../../es-419/.gitbook/assets/Failure Rate.png" alt=""><figcaption><p>Failure Rate Metric</p></figcaption></figure></div>

_**Example**: In this picture, the defined time frame was 1 week, divided into daily periods. Since this metric shows the failure rate, it is ideal for the results to be as low as possible. You will notice that, in this case, the failure rate was 0%, meaning that no requests failed during this period._

### Request Count

This metric represents the number of times the selected tag containers were requested within the defined time frame.

<div data-full-width="true"><figure><img src="../../../es-419/.gitbook/assets/request count.png" alt=""><figcaption><p>Request Count Metric</p></figcaption></figure></div>

_**Example**: A request is counted each time the tag container is rendered during your website's loading, according to your installation. In this picture, you can observe that the defined time frame was 1 week, divided into daily periods. Each line represents a different tag container selected from the list. For example, the blue line shows a little more than 1,000 daily requests on the first 4 days, then it decreased to nearly 400 requests on September 28th, and fluctuated between 400 and 700 requests for the rest of the week._
