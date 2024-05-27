---
description: >-
  In this page you will be learning how our metrics works in BMS platform and
  how to manage your Event Stores and Pipes Metrics.
---

# Metrics

All of our products have metrics in order to provide you with all the information we have once the product is being used.

## Visualization

We have two visualization options available:

* Metric Cards: This option displays your metrics on cards containing graphics. It's possible to export the data contained in each metric card by clicking on the desired card and then clicking on the download button <img src="../../.gitbook/assets/image (125).png" alt="" data-size="line">.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Event Stores - Metric Cards</p></figcaption></figure>

* Data Table: This option will bring the same data that are on the metric cards in table format. This visualization option allows you to export the data by clicking on the download button <img src="../../.gitbook/assets/image (125).png" alt="" data-size="line">.  You can also visualize the table in full-screen mode by clicking on ![](<../../.gitbook/assets/image (126).png>).

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption><p>Event Stores - Data Table</p></figcaption></figure>

## Time-Frames and Periodicity

One of the features on the metrics tab is defining a time frame and a period in which you want to visualize your metrics.

<div align="center">

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption><p>Metrics Tab - Period</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Captura de tela 2024-05-16 081812.png" alt=""><figcaption><p>Metrics Tab - Time Frame</p></figcaption></figure>

</div>

We can select a time frame to visualize the performance of any product's features within that period. To define a time frame, click on the button that represents the desired period or use the calendar button to set a custom time frame.

Additionally, it's also possible to set a period to define measurement intervals. For example, suppose you select a time frame of 1 day and a period of 1 hour. In that case, all the results from the last day will be displayed and divided into 1 hour periods.

To update your results click on the refresh button <img src="../../.gitbook/assets/image (122).png" alt="" data-size="original">.

## Event Stores

Once you start using our event stores, you will be able to check the metrics related to download data.

<figure><img src="../../.gitbook/assets/image (43).png" alt=""><figcaption><p>Grouped By Event Store Metrics</p></figcaption></figure>

You can also check your metrics grouping by **Type**, to separate your data by each event pipe's event.

<figure><img src="../../.gitbook/assets/image (48).png" alt=""><figcaption><p>Grouped by Type Metrics</p></figcaption></figure>

## Event Pipes

Once an event pipe is enabled and actions related to that event pipe are happening, the metrics will start updating.

You can group your metrics by Event Pipes, being able to compare your events and check how many events were matched.

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption><p>Grouped By Event Pipes</p></figcaption></figure>

You can also check each event pipe's target metrics, by grouping your metrics by **Targets**.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption><p>Grouped by Targets</p></figcaption></figure>

* Call Count - The number of times a target has been called for execution within the event pipe.
* Failure Rate - The ratio of failed execution attempts on a target within an event pipe.

When checking Metrics, you can always check our <img src="../../.gitbook/assets/image (28).png" alt="Information" data-size="line"> to receive more detailed information on how a specific metric works.
