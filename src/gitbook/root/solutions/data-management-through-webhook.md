---
description: Learn how to effectively use our Webhook Feature
---

# Data Management Through Webhook

### What is a Webhook

Webhooks are typically used to connect two different applications. When an event happens on the trigger application, it serializes data about that event and sends it to a webhook URL from the action application—the one you want to do something based on the data from the first application. The action application can then send a callback message.

Putting it in other words, when using a Webhook, all data provided by the first application will be sent automatically to a second application. Once the data reaches the second application, you can define how much of that data will be used, how and where the data will be placed, creating a fully customized data management.

In this solution, we will use a case where we want to collect data related to an Ad-Delivered event. From all data collected from that event, we will be using only **Time Stamp**, **Domain**, **Campaign ID**, and **Ad ID**, once we get that data, we will then create an action to send it to a Google Sheet.

The main reason for collecting that specific data is that we want to know the exact domain the user is receiving our banners and check if these domains are relevant to our campaign's target.

### Requirements

* Event Pipe or another feature that uses Webhook
* Zapier or any tool that has a Webhook feature
* Google Sheets
* Active Campaign

Follow the steps below to successfully manage your data through a webhook.

* [Creating an Event Pipe](data-management-through-webhook.md#creating-an-event-pipe)
* [Configuring your Webhook Tool](data-management-through-webhook.md#configuring-your-webhook-tool)
* [Trigger](data-management-through-webhook.md#trigger)
* [Action](data-management-through-webhook.md#action)
* [Start Collecting Data!](data-management-through-webhook.md#start-collecting-data)

### Creating an Event Pipe

To use a webhook, we will be using the Event Pipe feature to gather data from a running campaign.

Go to our Monitoring tab and click on **Event Pipes**.

<div align="center">

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Monitoring Tab</p></figcaption></figure>

</div>

There, we will be creating an event pipe by clicking on <img src="../.gitbook/assets/image (2).png" alt="Create Event Pipe" data-size="line">, in this case, we will be creating an ADS - Delivered event, so select the Sample event Template, our ADS - Delivered template.

<figure><img src="../.gitbook/assets/image (3).png" alt="" width="538"><figcaption><p>Event Pipe Screen</p></figcaption></figure>

Then click on <img src="../.gitbook/assets/image (5).png" alt="Add Filter" data-size="line"> to add a filter to collect data from ad-delivered events, by searching events that contain ad-delivered on their Type field.

<figure><img src="../.gitbook/assets/image (6).png" alt="" width="529"><figcaption><p>Event Pipe Filter</p></figcaption></figure>

Move to the Targets tab, there is where we configure our webhook link, click on <img src="../.gitbook/assets/image (8).png" alt="Add Target" data-size="line"> and then select Call Webhook.

<figure><img src="../.gitbook/assets/image (9).png" alt="" width="543"><figcaption><p>Create Target Screen</p></figcaption></figure>

Insert the URL provided by Zapier or your data management tool, and then **save** your Target and Event Pipe.

<figure><img src="../.gitbook/assets/image (17).png" alt="" width="542"><figcaption><p>Zapier Webhook Configured</p></figcaption></figure>

Make sure to have your Event Pipe enabled and an Active campaign to collect data and send it to your webhook tool.

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption><p>Event Pipe Enabled Tab</p></figcaption></figure>

### Configuring your Webhook Tool

For this solution we will be using Zapier as an example, but feel free to use your favorite data management tool, the only requirement is having a Webhook feature.

If you will be using Zapier as well, this is the link to access: [Zapier](https://zapier.com).

On Zapier, click on Create, then Zaps.

<figure><img src="../.gitbook/assets/image (11).png" alt="" width="221"><figcaption><p>Zapier Creation Menu</p></figcaption></figure>

We will then configure our trigger and action, based on Webhook + Event Pipe + Google Sheets.

<figure><img src="../.gitbook/assets/image (12).png" alt="" width="489"><figcaption><p>Zapier's Trigger and Action</p></figcaption></figure>

### Trigger

To configure our trigger, click on Trigger and then Search for Webhooks by Zapier.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption><p>Webhook Feature</p></figcaption></figure>

Then move to the App & Event Tab on your right, there you will configure your event to a Catch Hook event.

<figure><img src="../.gitbook/assets/image (15).png" alt="" width="404"><figcaption><p>Webhook Configuration</p></figcaption></figure>

Move to the Test Tab and get your **Webhook URL**.

<figure><img src="../.gitbook/assets/image (16).png" alt="" width="410"><figcaption><p>Webhook URL</p></figcaption></figure>

After configuring the webhook URL to your Event Pipe, click on Test Trigger to collect a data sample and use it to configure your Google Sheet.

{% hint style="warning" %}
_Attention! Make sure to have an **Active** Campaign and have your Event Pipe **enabled**, in order to have data available for that test._
{% endhint %}

The data might take a while to be available, once your event pipe sends information to your tool, this is the data you will get from that event.

<figure><img src="../.gitbook/assets/image (19).png" alt="" width="402"><figcaption><p>Zapier Data Collected</p></figcaption></figure>

Click on <img src="../.gitbook/assets/image (105).png" alt="" data-size="line"> and then we will move to configure the Action that will be taken after collecting the data.

If every step has been correctly followed, your Trigger will have a <img src="../.gitbook/assets/image (107).png" alt="Check" data-size="line"> informing that it is working as intended.

### Action

We will use **Google Sheets** to manage the data collected.

<figure><img src="../.gitbook/assets/image (106).png" alt="" width="377"><figcaption><p>Trigger and Action</p></figcaption></figure>

Create a Google sheet on your preferred account, and then have the Columns ready to be configured.

In this example, we will be collecting the following data: **Time Stamp**, **Domain**, **Campaign ID**, **Ad ID**.

<figure><img src="../.gitbook/assets/image (108).png" alt="" width="333"><figcaption><p>Google Sheet Configured</p></figcaption></figure>

We will be using the Create Spreadsheet Row Event on our Google sheet action configuration.

<figure><img src="../.gitbook/assets/image (109).png" alt="" width="410"><figcaption><p>Action Event Configuration</p></figcaption></figure>

After Configuring your account in the Account Tab, move to the Action tab.

There we will configure our Spreadsheet, worksheet and which data will be sent to each column.

<figure><img src="../.gitbook/assets/image (110).png" alt="" width="408"><figcaption><p>Spreadsheet and Worksheet Configured</p></figcaption></figure>

To better search each value, type on the search tab the value you want to collect.

<figure><img src="../.gitbook/assets/image (111).png" alt=""><figcaption><p>Data Collection</p></figcaption></figure>

After configuring all data fields with the collected sample from the **Trigger** test, you will be ready to start testing.



<figure><img src="../.gitbook/assets/image (112).png" alt="" width="400"><figcaption><p>Action Test</p></figcaption></figure>

Click on <img src="../.gitbook/assets/image (113).png" alt="" data-size="line"> and confirm that the data has been sent to your spreadsheet.

<figure><img src="../.gitbook/assets/image.png" alt="" width="563"><figcaption><p>Data Sent to Spreadsheet</p></figcaption></figure>

If every step has been followed successfully, your events will have a <img src="../.gitbook/assets/image (115).png" alt="Check" data-size="line">.

<figure><img src="../.gitbook/assets/image (116).png" alt="" width="251"><figcaption><p>Events Checked</p></figcaption></figure>

Click on <img src="../.gitbook/assets/image (117).png" alt="" data-size="line"> to enable your webhook and every data that is sent from our Event Pipe feature, will be available on your Google Sheets!

### Start Collecting Data!

Once you have an Active Campaign, Event Pipe and Webhook, this is how your Google Sheet will be updated.

<figure><img src="../.gitbook/assets/Spreadsheetdata Animated.gif" alt="" width="563"><figcaption><p>Google Sheet Real-Time Update</p></figcaption></figure>

{% hint style="info" %}
_If you are interested in more information about Webhooks through Zapier, here you can find more detailed information:_ [_Zapier Webhook Guide_](https://zapier.com/blog/what-are-webhooks/)
{% endhint %}

{% hint style="info" %}
_There are many tools that can be used to set up a Webhook, so find the tool that fits your needs. Zapier is just one of many options._
{% endhint %}
