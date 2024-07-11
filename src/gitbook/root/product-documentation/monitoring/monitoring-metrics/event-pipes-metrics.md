---
description: Learn more about how Event Pipes' metrics work.
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Event Pipes Metrics

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../../metrics.md).&#x20;
{% endhint %}

To access the metrics tab, select an Event Pipe and all metrics will be displayed, the metrics are populated once you have created event pipes and they are enabled and collecting data.

<figure><img src="../../../.gitbook/assets/image (272).png" alt=""><figcaption><p>Event Pipes Metrics</p></figcaption></figure>

### Matched Events Count

This metric is populated each time an event is matched to your event pipe's criteria, once it meets your configuration it collects data.

<figure><img src="../../../.gitbook/assets/image (273).png" alt=""><figcaption><p>Matched Events Count Metric</p></figcaption></figure>

_**Example:** Every time an event meets the criteria established during event pipe creation, this metric will be updated. It is important to monitor this metric, as it indicates whether the criteria are being correctly met; otherwise, there will be no data to collect. In this graph, you can see that at some point, it peaked at nearly 250,000 events. The metric will vary based on the number of campaigns running at the time._

### Target Execution Call Count

This metric is populated after the matched events succeed, every matched event will be sent to a target execution call, according to the criteria established, this metric will nearly always follow the same parameters as the matched event count.

<figure><img src="../../../.gitbook/assets/image (274).png" alt=""><figcaption><p>Target Execution Call Count Metric</p></figcaption></figure>

_**Example:** After an event matches the criteria, our system will execute the established event pipe, collect the data according to the parameters, and then send it to an event store or webhook, as configured. In this graph, you can see the matched event count._

### Target Execution Failure Rate

This metric is populated by the failures of a call execution, if there is any error instability on the platform or at the event pipe's configuration, our system will populate the failure rate metric.

<figure><img src="../../../.gitbook/assets/image (275).png" alt=""><figcaption><p>Target Execution Failure Rate Metric</p></figcaption></figure>

_**Example:** If a call execution fails, check your event pipe configuration or if the platform is experiencing instability, as this can cause the call execution to fail. In this graph, you can see that over the period of a month, there was a 1% failure rate on one day, followed by no failures afterward._

### Additional Information

These are all the metrics available in the Monitoring product for analyzing events. Additionally, when checking metrics, you can always check our <img src="../../../.gitbook/assets/image (28) (2).png" alt="Information" data-size="line"> to access additional information about a specific metric.
