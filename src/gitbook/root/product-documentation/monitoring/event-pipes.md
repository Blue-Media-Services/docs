---
description: Learn how to create and manage your Event Pipes.
---

# Event Pipes

Our Event Pipes are used to collect data from all products on our platform. You can use this feature to keep track of everything that can cause an event at BMS, from campaigns to organization creation, allowing you to organize the provided data as you wish.&#x20;

All event pipes created will be sent to either an Event Store, or you can use a webhook to send this data directly to your data management tool. We provide templates for every event that we can track so you can pick which you want to collect data.

{% hint style="info" %}
We have a solution that may help you understand how a webhook works, check this article [here](../../solutions/data-management-through-webhook.md).
{% endhint %}

## Creating an Event Pipe

To create an event store, click on <img src="../../.gitbook/assets/image (9).png" alt="Create Event Pipe" data-size="line"> , and an event pipe creation screen will pop up.

<figure><img src="../../.gitbook/assets/image (10).png" alt="" width="541"><figcaption><p>Event Pipe Creation</p></figcaption></figure>

* Name - Set a name for your Event Store.
* Tags - Create tags to better identify each event pipe.

### Filters

To start configuring your event pipe, pick a template of your choice in our Filters tab according to your needs.

* Sample Event Template - In this dropdown menu, you will be provided with all templates related to the events that we can track.

In this example, we will be creating an event pipe for ADS - Delivered. This event tracks every Ad that is currently running in a campaign and is delivering impressions. Once we create this event pipe, all data will be sent to an Event Store or a Webhook.

<figure><img src="../../.gitbook/assets/image (11).png" alt="" width="529"><figcaption><p>ADS - Ad Delivered Event Pipe</p></figcaption></figure>

Once we have the template selected, you can check which data will be collected when creating the corresponding Event Pipe.

To collect the data, we **must** insert a filter, by clicking on ![Add Filter](<../../.gitbook/assets/image (12).png>).

<figure><img src="../../.gitbook/assets/image (13).png" alt="" width="515"><figcaption><p>Adding Filters</p></figcaption></figure>

* Path - Specific tag in which you can identify the event. Ex: id, type, source, data.accountId.
* Operator - Rule that will be used on this filter,
* Value - Which specific value the tag must contain.

In this case, we will be collecting data from ad-delivered events, so this is how the configuration would look.

<figure><img src="../../.gitbook/assets/image (14).png" alt="" width="524"><figcaption><p>Event Pipe Filter Settings</p></figcaption></figure>

We specified the **Path** using the tag "Type", chose the **Operator** option to "Contains" and added the **Value** "Ad-delivered". Note that these fields are case sensitive, so the fulfilled fields **must** match the template.

Once you have fulfilled all fields with the corresponding information based on your event pipe, the test filter must have a check confirming that it is working properly <img src="../../.gitbook/assets/image (15).png" alt="Test Filters Checked" data-size="line">. If it is not working properly due to missing information or a typo, it will be presented with a warning sign <img src="../../.gitbook/assets/image (17).png" alt="Test Filters Warning" data-size="line">.

<figure><img src="../../.gitbook/assets/image (16).png" alt="" width="518"><figcaption><p>Test Filter Warning</p></figcaption></figure>

In this case, our filter failed due to verification in our Value field.  These fields are case-sensitive and **must** match the corresponding information.

Once you have added your filters, move to the targets tab.

### Targets

Here you will be deciding where you will send the data to, whether it will be sent to one or multiple event stores, or to a webhook.

<figure><img src="../../.gitbook/assets/image (18).png" alt="" width="537"><figcaption><p>Event Pipe's Targets Tab</p></figcaption></figure>

To configure a target, click on ![Add Target](<../../.gitbook/assets/image (19).png>).

<figure><img src="../../.gitbook/assets/image (20).png" alt="" width="350"><figcaption><p>Event Store Target</p></figcaption></figure>

If you decide to send your data to an event store, simply name your target and choose your already created event store.

<figure><img src="../../.gitbook/assets/image (21).png" alt="" width="357"><figcaption><p>Call Webhook Target</p></figcaption></figure>

It is possible to send your data to a webhook, provided by your data management tool, this is an option if you already have a data management tool of preference.

After making all necessary changes, click on <img src="../../.gitbook/assets/image (22).png" alt="Save" data-size="line"> to create your target.

<figure><img src="../../.gitbook/assets/image (23).png" alt="" width="533"><figcaption><p>Event Pipe Target Created</p></figcaption></figure>

Once everything is configured, click on <img src="../../.gitbook/assets/image (22).png" alt="Save" data-size="line"> and your event pipe will be listed.

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption><p>Event Pipes List</p></figcaption></figure>

### Enabling your Event Pipe

To enable an event pipe simply flip the toggle <img src="../../.gitbook/assets/image (33).png" alt="Toggle" data-size="line"> and your event store will be enabled.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Event Pipe Enabled</p></figcaption></figure>

### Editing your Event Pipe

To edit your event store, click on <img src="../../.gitbook/assets/image (35).png" alt="Edit" data-size="line"> and an editing screen will pop up, make the necessary changes and then click on <img src="../../.gitbook/assets/image (32).png" alt="Save" data-size="line">.

<figure><img src="../../.gitbook/assets/image (3).png" alt="" width="527"><figcaption><p>Event Pipe's Edit Screen</p></figcaption></figure>

### Bulk Actions

When selecting two or more event pipes, the Bulk Actions will be enabled, allowing you to make actions in bulk.

You will be capable of Archiving and Deleting events in bulk.

<figure><img src="../../.gitbook/assets/image (2) (6).png" alt=""><figcaption><p>Event Pipe's Bulk Actions</p></figcaption></figure>

### Archiving and Unarchiving your Event Pipe

To archive your event pipe, click on <img src="../../.gitbook/assets/image (37).png" alt="Archive" data-size="line"> and it will be sent to the archived list. In order to unarchive your event pipe, switch your view to archived events by flipping the toggle <img src="../../.gitbook/assets/image (38).png" alt="Archived Toggle" data-size="line">. You will then be presented with the list of archived events. Click on <img src="../../.gitbook/assets/image (39).png" alt="Unarchive" data-size="line"> to unarchive an event pipe.

### Deleting your Event Pipe

To delete an event, click on ![](<../../.gitbook/assets/image (138).png>) and a confirmation will be required.

<figure><img src="../../.gitbook/assets/image (131).png" alt=""><figcaption><p>Event Pipe Deletion</p></figcaption></figure>

After clicking on <img src="../../.gitbook/assets/image (140).png" alt="Delete" data-size="line">, your event pipe will be deleted.

{% hint style="warning" %}
_We advise users to archive instead of deleting, only delete if you are sure of it, the action cannot be undone._
{% endhint %}
