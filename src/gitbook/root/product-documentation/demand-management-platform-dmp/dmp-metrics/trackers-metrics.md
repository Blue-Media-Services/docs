---
description: Learn more about how trackers metrics work.
---

# Trackers Metrics

{% hint style="info" %}
To learn more about how the metrics service works, how to set your visualization options, and how to download your data, visit our [Metrics page](../../metrics.md).&#x20;
{% endhint %}

To access the metrics tab select the trackers which you want to visualize data on the trackers' list:

<figure><img src="../../../.gitbook/assets/image (120).png" alt=""><figcaption><p>Trackers' Metrics Tab</p></figcaption></figure>

You can select more than one tracker. However, the 'Group by' optionis only available when selecting a single tracker. When selecting multiple trackers, the data will be grouped by tracker and this option will not be displayed.

## Grouping by Tracker

When grouping by tracker all the data collected by the selected tracker will be displayed on these metric cards or in the data table columns:

### **Action Execution Count**

This metric shows how many actions were executed by your tracker on the configured time frame.

<figure><img src="../../../.gitbook/assets/image (261).png" alt=""><figcaption></figcaption></figure>

_**Example:** On this graph, you can observe an increase in the number of actions at 6 AM. The graph displays a time frame of 3 hours divided into 5-minute intervals represented as data points. After creating a tracker, you will need to set up events and actions. Each time a tracked event occurs, the configured actions associated with that event will also be executed. For instance, an 'add to cart' event might trigger an action to track the added product in the catalog. This metric indicates when and how often the action is executed within that time frame._

### **Action Failure Rate**

This metric shows when an event has been tracked, however, the action linked to it has failed.

<figure><img src="../../../.gitbook/assets/image (262).png" alt=""><figcaption></figcaption></figure>

_**Example:** When a user adds a product to their cart on your website and this event is configured to be tracked, with an action to track it in the catalog, the event itself was tracked successfully. However, the action to update the catalog failed, resulting in the product not being tracked. In the graph, you can observe that the action failure rate is typically 0%. However, there are moments where the action failure rate peaks near 40%. The graph covers a time frame of 3 hours, divided into 5-minute intervals represented as data points._

### **Expiration Count**

This metric shows the amount of users' expirations that occurred in the defined time frame.

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

_**Example:** When configuring a tracker, you can set a tracking period after which the user will expire. This metric shows the number of expirations that occurred. On this graph, you can observe that between 4 AM and 5 AM, nearly 50 tracked users expired._

### **Maximum Users**

This metric shows the configured maximum number of users to be added to the tracker.

<figure><img src="../../../.gitbook/assets/image (264).png" alt=""><figcaption></figcaption></figure>

_**Example:** When creating or editing a tracker, you will set the maximum number of users allowed to be added to your tracker. This metric displays that data. In this graph, you can observe that the tracker was configured to accept up to 1 million users_

### **New Activities**

Whenever a user performs a new tracked activity on your website, this will be tracked,  this metric will show the number of new activities tracked in a defined time frame.

<figure><img src="../../../.gitbook/assets/image (265).png" alt=""><figcaption></figcaption></figure>

_**Example:** You have an 'add to cart' event configured on your tracker. Whenever a user adds a product to the cart, it counts as a new activity. On this graph, you will notice that the number of new activities increases after 6 AM. You will also observe that this graph covers a time frame of 3 hours, divided into 5-minute intervals represented as data points._

### **Time Until Expiration**

This metric shows the remaining time a cookie is still available in the pool until expiring in the determined time frame.

<figure><img src="../../../.gitbook/assets/image (267).png" alt=""><figcaption></figcaption></figure>

_**Example:** When you create your cookie pool you can set the number of days in which a cookie will expire, this metric shows you how much time you have until a cookie expiration. On this graph, the time frame was of 1 week, divided into daily periods, represented as dots, you can observe that on June 20th there was less than 1 day until some of the cookies in the pool expire._

### **Tracker User Count**

This metric will show how many users were in the tracker in the defined time frame.

<figure><img src="../../../.gitbook/assets/image (268).png" alt=""><figcaption></figcaption></figure>

_**Example:** After setting up a tracker on your website, your website's users will begin to be tracked. The number of users tracked within a defined time frame is the data shown in this metric. On this graph, you will notice that the number of tracked users between 4 AM and 6 AM was nearly 400 thousand._

## Grouping by Event&#x20;

<figure><img src="../../../.gitbook/assets/image (127).png" alt=""><figcaption><p>Trackers' Metrics tab - Grouped by Event</p></figcaption></figure>

When grouping by event, the displayed metrics will be separated according to their respective events. The following metric cards or data table columns are available:

### **Action Execution Count**

This metric shows the number of actions executed by each tracked event within the configured time frame.

<figure><img src="../../../.gitbook/assets/image (269).png" alt=""><figcaption></figcaption></figure>

_**Example:** You have a 'product view' event configured on your tracker, linked to a 'track in catalog' action. Every time a product is viewed, the event is tracked, and the associated action is executed. This metric shows this data grouped by event. On this graph, you can observe an increase in actions around 6 AM. The graph covers a time frame of 3 hours, divided into 5-minute intervals represented as data points._

### **Action Failure Rate**

This metric shows instances where an event was tracked but the linked action failed to execute. The data is displayed grouped by event.

<figure><img src="../../../.gitbook/assets/image (271).png" alt=""><figcaption></figcaption></figure>

_**Example:** When a user on your website adds a product to the cart and this event is configured to be tracked, with an action to track it in the catalog, the event is successfully tracked. However, the action fails to execute, resulting in the product not being tracked in the catalog. On this graph, you can see that the action failure rate is typically 0%, but there are moments where it reaches nearly 40%. The graph covers a time frame of 3 hours, divided into 5-minute intervals represented as data points._

### **New Activities**

Whenever a user performs a new tracked activity on your website, it will be recorded. This metric shows the number of new activities tracked within a defined time frame, grouped by event.

<figure><img src="../../../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>

_**Example:** You have 'add to cart' and 'product view' events configured on your tracker. Every time a user performs any of these tracked activities, it will be counted and displayed in this metric, grouped by event. On this graph, you will notice that the number of new activities increases after 6 AM. The graph covers a time frame of 3 hours, divided into 5-minute intervals represented as data points._

These are all the metrics available in the DMP product for analyzing the performance of your cookie pools and trackers. Additionally, when checking metrics, you can always check our <img src="../../../.gitbook/assets/image (28) (2).png" alt="Information" data-size="line"> to access for more information about a specific metric.
