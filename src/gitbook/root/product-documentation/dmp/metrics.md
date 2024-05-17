---
description: Learn about the DMP features' metrics tab.
---

# Metrics

Trackers and Cookie Pools have their own metrics tab, bringing us data about their performance and behavior.

## Cookie Pools

Select a cookie pool on the list above to access its metrics, it's also possible to select more than one to compare their results between them.

There are 2 visualization options available:

### Metric Cards

This option will show your cookie pools' results as cards containing graphics:

<figure><img src="../../.gitbook/assets/image (123).png" alt=""><figcaption><p>Cookie Pools' Metrics Tab - Metrics Cards Visualization</p></figcaption></figure>

Each card contains relevant data about your cookie pools:

* Expiration Count: The amount of cookies that expired.
* Max Size: Maximum amount of cookies allowed in the pool.
* Size: The amount of cookies inside the pool.
* Sync Count: The amount of cookies synchronizations.
* Time Until Expiration: The amount of time a cookie will be available in the pool before expiring.

It's possible to export the data contained on each metric card by clicking on the desired card and then clicking on the download button <img src="../../.gitbook/assets/image (125).png" alt="" data-size="line">, after selecting the desired time frame.

### Data Table

This option will bring the same data that are on the metric cards in table format:

<figure><img src="../../.gitbook/assets/image (124).png" alt=""><figcaption><p>Cookie Pools' Metric Tab - Data Table Visualizitation</p></figcaption></figure>

This visualization option allows you to export the data by clicking on the download button <img src="../../.gitbook/assets/image (125).png" alt="" data-size="line">, you can also visualize the table in full-screen mode by clicking on ![](<../../.gitbook/assets/image (126).png>).

## Trackers

To access the metrics tab select the trackers which you want to visualize data on the trackers' list:

<figure><img src="../../.gitbook/assets/image (120).png" alt=""><figcaption><p>Trackers' Metrics Tab</p></figcaption></figure>

We can select more than one tracker, however, the option 'Group by' is only available when selecting only one tracker, when selecting more than one tracker, the data will be grouped by tracker and this option won't be displayed.

The available visualization options are the same as the ones we have for the cookie pools and work equally.

### Grouping by Tracker

When grouping by tracker all the data collected by the selected tracker will be displayed on these metric cards or data table columns:

* Action Execution Count: Number of times an action was executed.
* Action Failure Rate: The rate of action failures.
* Expiration Count: The number of user expirations.
* Maximum Users: Maximum number of users to be added to the tracker.
* New Activities: Number of new activities tracked.
* Time Until Expiration: The amount of time the users tracked remains available before expiring.
* Tracker User Count: The number of users tracked.

### Grouping by Event&#x20;

<figure><img src="../../.gitbook/assets/image (127).png" alt=""><figcaption><p>Trackers' Metrics tab - Grouped by Event</p></figcaption></figure>

When grouping by event the displayed metrics will be separated according to the event to which they belong, these are the available metric cards or data table columns:

* Action Execution Count: Number of times an action was executed.
* Action Failure Rate: The rate of action failures.
* New Activities: Number of new activites tracked.

## Time-frames and Periodicity

One of the features on the metrics tab is defining a time frame and a period in which you want to visualize your trackers and cookie pools performances.&#x20;

<div align="center">

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption><p>Metrics Tab - Period</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Captura de tela 2024-05-16 081812.png" alt=""><figcaption><p>Metrics Tab - Time Frame</p></figcaption></figure>

</div>

We can select a time frame to visualize the data collected by our trackers or cookie pools on this time frame. To define a time frame, you can click on the button that represents the time frame you want or use the calendar button to define a customized time frame.

Additionally, it's also possible to set a period to define measurement time. For example, suppose you select a time frame of 1 day and a period of 1 hour. In that case, all the results on the last day will be displayed and divided into 1 hour periods, so you can gather knowledge about what hours of the day your users are more active.

To update your results click on the refresh button <img src="../../.gitbook/assets/image (122).png" alt="" data-size="original">.
