---
description: Learn more about how Event Stores Metrics work.
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

# Event Stores Metrics

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../../metrics.md).&#x20;
{% endhint %}

Select an event store to check the metrics populated by the event pipes, note that it is necessary to use an event store to populate when creating an event pipe, if you send your events only to a webhook, the event store will not be populated.

<figure><img src="../../../.gitbook/assets/image (276).png" alt=""><figcaption><p>Event Stores Metrics</p></figcaption></figure>

### Stream Bytes

It Is populated by having Event Streams available for download, according to the size of each event stream, this metric will present the sum of all your event streams' bytes.

<figure><img src="../../../.gitbook/assets/image (3) (1) (1) (1) (1).png" alt=""><figcaption><p>Stream Bytes Metric</p></figcaption></figure>

_**Example:** After having an event store populated, it will present event streams related to the pipes selected. Then you will be able to check the size and date of each pipe separately. The graph will populate as the stream's size increases. It is possible to see on this graph that it reached nearly 2 MB in size within a week._

### Stream Count

It presents the count of each event stream presented on your event store, if the event store has many pipes related to it, the count will be high.

<figure><img src="../../../.gitbook/assets/image (4) (1) (1) (1).png" alt=""><figcaption><p>Stream Count Metric</p></figcaption></figure>

_**Example:** When creating event pipes, you must select an event store or a webhook to send the data. Once you select an event store, each pipe you create to the same event store will generate an event stream when receiving data. It is important to note that if you have too many event pipes to the same event store, it is advisable to separate them in order to better organize your event streams. On this graph, you can see that the stream count reached a peak of nearly 200 streams._

### Stream Upload Bytes

Presents the total amount of bytes uploaded to your event streams tab, leaving streams available for download.

<figure><img src="../../../.gitbook/assets/image (25) (1).png" alt=""><figcaption><p>Stream Upload Bytes Metric</p></figcaption></figure>

_**Example:** Each event stream is uploaded to your selected event store after a few minutes, being available for download as a .JSON file. The metric will present the sum of all uploaded event streams' bytes to your event store. On this graph, we can see that on specific dates, the data was significantly reduced due to the expiration date of each event stream or deletion._

### Stream Upload Count

This metric presents the total upload count, related to each event stream's data collected and presented for download, once they expire or get deleted, the count will decrease.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Stream Upload Count Metric</p></figcaption></figure>

_**Example:** On this graph, it is possible to see that on some dates the count reached nearly zero due to having no active event pipes or because of a cleanup. It is important to check your upload count since it might impact how you are organizing your event streams. Having too many event streams to organize can be confusing, so a cleanup or optimization should be done from time to time._

### Stream Download Bytes

This metric represents the sum of all downloaded bytes of your event streams and will be populated only when the event stream has been downloaded.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption><p>Stream Download Bytes Metric</p></figcaption></figure>

_**Example:** Once you start downloading your event streams' data, you will be informed of the total number of bytes downloaded each day. This helps you keep track of how much data was downloaded. If the data volume is high, it indicates that many events were captured from the event stream. In this graph, you can see that only 2 KB of data was downloaded._

### Stream Download Count

This metric represents the event streams downloaded, which will be populated every time you download an event stream.

<figure><img src="../../../.gitbook/assets/image (5) (1) (1) (1).png" alt=""><figcaption><p>Stream Download Count Metric</p></figcaption></figure>

_**Example:** If you organize yourself to download the collected event pipe data every week or every two weeks, the metric will inform you so that you don't lose track of your established schedule. In this graph, you can see that the event streams were downloaded only after a week._

### Stream Delete Bytes

This metric is populated every time an event stream is deleted by showing you the sum of all bytes deleted, either manually or by the retention date set upon event store creation.

<figure><img src="../../../.gitbook/assets/image (6) (1) (1).png" alt=""><figcaption><p>Stream Delete Bytes Metric</p></figcaption></figure>

_**Example:** Once you start collecting data for your event store, you will set a retention date for the data. Every time the data reaches that date, your event stream will be deleted, or you can also delete it manually. In this graph, you can see that, at some point, nearly all event streams were deleted._

### Stream Delete Count

This metric represents the total count of deleted event streams, they are populated either by retention deletion or manual deletion.

<figure><img src="../../../.gitbook/assets/image (7) (1) (1).png" alt=""><figcaption><p>Stream Delete Count Metric</p></figcaption></figure>

_**Example:** On this graph, you can see that the delete count follows a pattern, but on some dates, a lower amount was deleted. This could be due to a change in the retention date or fewer event streams being enabled. Deleting data can help you keep it more organized._

### Additional Information

These are all the metrics available in the Monitoring product for analyzing events. Additionally, when checking metrics, you can always check our <img src="../../../.gitbook/assets/image (28) (2).png" alt="Information" data-size="line"> to access additional information about a specific metric.
