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

# Event Stores

In our Event Stores tab, you can create a store that acts as a database for storing events. You will be able to create a store where your event pipes will be sent. You can then download the events as a JSON file and import that to your data management file to organize it better.

<figure><img src="../../.gitbook/assets/image (29) (2).png" alt="" width="563"><figcaption><p>Event Stores Tab</p></figcaption></figure>

## Creating an Event Store

To create an event store, click on ![Create Event Store](<../../.gitbook/assets/image (3).png>) then an event creation screen will pop up.

<figure><img src="../../.gitbook/assets/image (31) (2).png" alt="" width="361"><figcaption><p>Event Store Creation</p></figcaption></figure>

* Name - Set a name for your Event Store.
* Tags - Create tags to better identify each event store.
* Retention - Decide for how long you will be keeping the data collected by this event store, after expiration, the data will be **deleted**.

After configuring your event store, click on ![Save](../../.gitbook/assets/image.png) button to finish your event creation.

### Enabling your Event Store

To enable an event store simply flip the toggle <img src="../../.gitbook/assets/image (33) (2).png" alt="Toggle" data-size="line"> and your event store will be enabled.

<div align="center"><figure><img src="../../.gitbook/assets/image (34) (2).png" alt="" width="148"><figcaption><p>Event Store Enabled</p></figcaption></figure></div>

### Editing your Event Store

To edit your event store, click on <img src="../../.gitbook/assets/image (35) (2).png" alt="Edit" data-size="line"> and an editing screen will pop up, make the necessary changes, and then click on ![Save](../../.gitbook/assets/image.png).

<figure><img src="../../.gitbook/assets/image (36) (2).png" alt="" width="360"><figcaption><p>Edit Event Store Screen</p></figcaption></figure>

### Bulk Actions

When selecting two or more event stores, the Bulk Actions will be enabled, allowing you to make actions in bulk.

You will be capable of Archiving, Deleting, Enabling, and Disabling events in bulk.

<figure><img src="../../.gitbook/assets/image (1) (8).png" alt=""><figcaption><p>Event Stores' Bulk Actions</p></figcaption></figure>

### Archiving and Unarchiving your Event Store

To archive your event store, click on <img src="../../.gitbook/assets/image (37) (2).png" alt="Archive" data-size="line"> and your event store will be sent to the archived list. In order to unarchive your event store, switch your view to archived events by flipping the toggle <img src="../../.gitbook/assets/image (38) (2).png" alt="Archived Toggle" data-size="line">. You will then be presented with the list of archived events. Click on <img src="../../.gitbook/assets/image (39).png" alt="Unarchive" data-size="line"> to unarchive an event store.

### Deleting your Event Store

To delete an event store, click on <img src="../../.gitbook/assets/image (40).png" alt="Delete" data-size="line"> and a confirmation screen will pop up.

<figure><img src="../../.gitbook/assets/image (41).png" alt="" width="359"><figcaption><p>Deletion Screen</p></figcaption></figure>

To confirm your deletion click on ![Delete](<../../.gitbook/assets/image (2).png>).

{% hint style="danger" %}
_Attention! If you delete an event store, all data related to that event store will be deleted._
{% endhint %}

## Event Streams

Once you create your event stores and pipes, all triggered events will be presented on your Event Streams tab, being available for download according to your data retention settings.

These data will **only** be displayed if there is an event pipe sending data to an event store.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-28 072309.png" alt=""><figcaption><p>Event Streams Tab</p></figcaption></figure>

### Downloading your Event Streams

You are able to download your event streams by clicking on ![](<../../.gitbook/assets/image (6) (11).png>) at the same row as the event stream you want to download. There are two formats of files available:

#### JSON-line

The JSON-line format offers a raw and unfiltered view of the event stream, capturing all relevant information as events occur. This format ensures that no data is left out, giving you complete visibility into each transaction for detailed analysis or integration into custom workflows.

<figure><img src="../../.gitbook/assets/image (1) (16).png" alt=""><figcaption><p>JSON-line</p></figcaption></figure>

Select this format and then click on ![Download](<../../.gitbook/assets/image (4).png>) to download your event stream.

#### CSV

The CSV format provides a customizable and organized view of the event stream, enabling you to choose specific data fields for export. This format makes the data easier to analyze in spreadsheet applications or reporting tools while retaining essential information needed for insights into advertising performance and activity.

<figure><img src="../../.gitbook/assets/image (4) (9).png" alt=""><figcaption><p>CSV</p></figcaption></figure>

It is possible to add or remove columns to your CSV file. To add a column click on <img src="../../.gitbook/assets/image (6) (11) (1).png" alt="" data-size="line">, and then fill in the details:

<figure><img src="../../.gitbook/assets/image (5) (10) (1).png" alt=""><figcaption><p>Add Column</p></figcaption></figure>

* Label - Inform the desired label for the column
* Read Data From - Inform the parameter from where you want to read data
* Default Value - Fill this with a default value for the column, this field is optional.

To remove a column, select it in the list and then click at ![](<../../.gitbook/assets/image (7) (11).png>).

After finishing your settings, click on ![Download](<../../.gitbook/assets/image (4).png>) to download your CSV file.

### Bulk Actions

You can select multiple event streams by checking the <img src="../../.gitbook/assets/image (133).png" alt="Checkbox" data-size="line">, after selecting more than one event, the bulk options will enable, you can download the selected event streams by clicking on <img src="../../.gitbook/assets/image (9) (10).png" alt="" data-size="line">, and selecting one of the file formats available.

It's also possible to bulk delete your event streams, click on <img src="../../.gitbook/assets/image (10).png" alt="" data-size="line">, then select delete, and confirm the deletion when it is asked.

### Deleting Event Streams

To delete an event, click on ![](<../../.gitbook/assets/image (138).png>) and a confirmation will be required.

<figure><img src="../../.gitbook/assets/image (139).png" alt="" width="359"><figcaption><p>Event Deletion</p></figcaption></figure>

After clicking on ![Delete](<../../.gitbook/assets/image (2).png>), your event data will be permanently deleted.

{% hint style="danger" %}
_Attention! Be careful when deleting event streams, this action cannot be undone, meaning, your data is permanently removed._
{% endhint %}
