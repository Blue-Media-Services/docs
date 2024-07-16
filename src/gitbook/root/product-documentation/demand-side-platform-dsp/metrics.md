---
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

# DSP Metrics

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../metrics.md).&#x20;
{% endhint %}

You can have a more precise view of your campaign by checking the <img src="../../.gitbook/assets/image (32) (1).png" alt="Overview" data-size="line"> tab. Here you will be presented with the most valuable metrics of a campaign, which can be divided by **Targets**, **Ads**, **Creative Groups**, and **Creatives**.

<figure><img src="../../.gitbook/assets/image (34) (1).png" alt=""><figcaption><p>Campaign Overview</p></figcaption></figure>

It is possible to select a campaign and then choose a specific date to view the overview for that period.

After selecting a campaign and a period, you will be presented with an overview of that campaign, including all targets, ads, creative groups, and creatives that are impacting the campaign, and how they are performing.

<figure><img src="../../.gitbook/assets/image (229).png" alt=""><figcaption><p>Overview Display</p></figcaption></figure>

Alternatively, in the Campaigns section, a metrics tab is available containing the same data, but following our metrics standard. When not selecting any of your campaigns, this tab will show you an account-wide of all your campaigns. Selecting more than one campaign will show a comparison between the selected campaigns, and selecting only one campaign will enable the group by feature with four options:

* **Campaign**: This option will display all the available metrics for the selected campaign.
* **Ad**: This option will display a data comparison between the ads on the selected campaign, allowing you to gather information about your audience. This information can be used to create more engaging ads in the future.
* **Target:** This option will display a data comparison between your campaign's targets, allowing you to gather information about your audience. This information can be used to configure more precise targets in the future.
* **Exchange**: This option will display a data comparison between the ad exchanges used to run your campaign, allowing you to gather data on which ad exchange has been more effective for your campaign.

<figure><img src="../../.gitbook/assets/image (230).png" alt=""><figcaption><p>Campaign Metrics Tab - Grouped by Campaing</p></figcaption></figure>

The ads metrics are also available on this page, they are: budget spent, bids, bid win, impressions, CPM, deliveries, delivery (%), displays, display (%), views, viewability, clicks, CTR, CPC, time to display, time to view, time to click, bid price effective, impressions price, budget spent on impressions and budget spent on deliveries. You can learn more about these metrics on the [Ads Metrics](../ad-server/ads/ads-metrics.md) page. This article is dedicated to discussing the exclusive campaign metrics:

### Campaign Active

This metric indicates whether your campaign has been active or not, and when the campaign has been active within the selected time frame.

<figure><img src="../../.gitbook/assets/image (231).png" alt=""><figcaption><p>Campaign Active Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe that the campaign has been active during the period June 16-24. This metric shows results only when a campaign has been active. If there are no results in this metric, it means that the campaign was disabled during that period._

### Bid Price Target

This metric shows the bid price configured for your campaign. There are three visualization options: minimum, maximum, and average. The displayed value is for 1,000 bids

<figure><img src="../../.gitbook/assets/image (232).png" alt=""><figcaption><p>Bid Price Target Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe that the average bid price for this campaign was $50 per bid for the defined time frame (June 17-24). If you set a variable bid price between $0,0001 and $100 you will observe that this metric will show you the bid price targeted, on the maximum visualization you will see the card shows the maximum bid value, on the minimum, it shows the minimum value, and on the average, the average value configured for your campaign._

### Device Count

This metric shows the number of unique devices from which you have received an impression. Each device is counted only once.

<figure><img src="../../.gitbook/assets/image (233).png" alt=""><figcaption><p>Device Count Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe that the ad was delivered to 4 different devices on June 17th, to 3 devices on June 18th-19th, and 1 device per day until the end of the defined time frame ( June 17-24). If a user inside the parameters of your target receives your ads on his PC, this will count as a unique device, if the same user receives your ads on his smartphone it will count as another device._

### Device Frequency

This metric displays how many impressions your ads receive from the same device.

<figure><img src="../../.gitbook/assets/image (234).png" alt=""><figcaption></figcaption></figure>

_**Example:** A user within your target parameters can be impacted multiple times by the same ad on the same device. This metric counts how many times the ad was displayed on the same device. In this graph, you can observe that on June 17th, your ad was delivered to the same device just over 10 times, while on June 18th, this number increased to about 15 times per device._

### Budget Spent with Recommendations

This metric shows how much of your budget was spent based on recommendations. It will only appear if you are using a recommendation model for this campaign.

<figure><img src="../../.gitbook/assets/image (224) (1).png" alt=""><figcaption><p>Budget Spent with Recommendations Metric</p></figcaption></figure>



_**Example:** In a context where you have a retargeting campaign designed to engage users on your website, the budget allocated to recommending products from your catalog to these users is shown in the "Budget spent on recommendations" metric. The graph displays a one-week time period, with each point corresponding to a day and the budget spent on recommendations. You can see that on June 24th, the budget spent on recommendations was almost $0.07, with a considerable drop on June 28th._

### Budget Pace Target

This metric shows the defined budget pace target. It helps you plan the rate at which your budget will be consumed.

<figure><img src="../../.gitbook/assets/image (235).png" alt=""><figcaption><p>Budget Pace Target Metric</p></figcaption></figure>

_**Example:** If you have a daily budget of $10, this metric will show the pace at which this budget should be spent over the course of your campaign. In this graph, you can observe that the daily budget was under $5 from June 16th to June 23rd, then on June 24th, the daily budget increased to $15._

### Budget Pace Effective

This metric shows you the actual race at which your budget is being consumed. It allows you to gather information on which hours of the day or days of the week, your ads spent your budget.

<figure><img src="../../.gitbook/assets/image (225) (1).png" alt=""><figcaption><p>Budget Pace Effective Metric</p></figcaption></figure>



_**Example:** In this graph, you can observe the budget pace adjusted to spend all the budget defined for that period (June 21-24). The budget pace effective metric will show you how this budget is being spent effectively and during which hours or days it has been spent._

### Budget Available

This metric shows how much of your budget is still available for a campaign, it will show new values as the budget is being spent.

<figure><img src="../../.gitbook/assets/image (226).png" alt=""><figcaption><p>Budget Available Metric</p></figcaption></figure>

_**Example:** In this graph, you can see that there was a daily budget of $30, which was completely spent each day from June 21st until June 24th. By following this metric, you will be able to observe how much of your budget remains available for your campaign._

### Additional Information

These are all the metrics available in the campaign product for analyzing the performance of your campaign.  Additionally, when checking metrics, you can always check our <img src="../../.gitbook/assets/image (28) (2).png" alt="Information" data-size="line"> to access additional information about a specific metric.
