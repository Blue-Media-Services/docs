# Almacenamiento de Eventos

In our Event Stores tab, you can create a store that acts as a database for storing events. You will be able to create a store where your event pipes will be sent. You can then download the events as a JSON file and import that to your data management file to organize it better.

<figure><img src="../../.gitbook/assets/image (210).png" alt="" width="563"><figcaption><p>Event Stores Tab</p></figcaption></figure>

## Creating an Event Store

To create an event store, click on ![Create Event Store](<../../.gitbook/assets/image (977).png>) then an event creation screen will pop up.

<figure><img src="../../.gitbook/assets/image (422).png" alt="" width="361"><figcaption><p>Event Store Creation</p></figcaption></figure>

* Name - Set a name for your Event Store.
* Tags - Create tags to better identify each event store.
* Retention - Decide for how long you will be keeping the data collected by this event store, after expiration, the data will be **deleted**.

After configuring your event store, click on ![Save](<../../.gitbook/assets/image (974).png>) button to finish your event creation.

### Enabling your Event Store

To enable an event store simply flip the toggle <img src="../../.gitbook/assets/image (424).png" alt="Toggle" data-size="line"> and your event store will be enabled.

<div align="center"><figure><img src="../../.gitbook/assets/image (425).png" alt="" width="148"><figcaption><p>Event Store Enabled</p></figcaption></figure></div>

### Editing your Event Store

To edit your event store, click on <img src="../../.gitbook/assets/image (426).png" alt="Edit" data-size="line"> and an editing screen will pop up, make the necessary changes, and then click on ![Save](<../../.gitbook/assets/image (974).png>).

<figure><img src="../../.gitbook/assets/image (427).png" alt="" width="360"><figcaption><p>Edit Event Store Screen</p></figcaption></figure>

### Bulk Actions

When selecting two or more event stores, the Bulk Actions will be enabled, allowing you to make actions in bulk.

You will be capable of Archiving, Deleting, Enabling, and Disabling events in bulk.

<figure><img src="../../.gitbook/assets/image (180).png" alt=""><figcaption><p>Event Stores' Bulk Actions</p></figcaption></figure>

### Archiving and Unarchiving your Event Store

To archive your event store, click on <img src="../../.gitbook/assets/image (428).png" alt="Archive" data-size="line"> and your event store will be sent to the archived list. In order to unarchive your event store, switch your view to archived events by flipping the toggle <img src="../../.gitbook/assets/image (429).png" alt="Archived Toggle" data-size="line">. You will then be presented with the list of archived events. Click on <img src="../../.gitbook/assets/image (876).png" alt="Unarchive" data-size="line"> to unarchive an event store.

### Deleting your Event Store

To delete an event store, click on <img src="../../.gitbook/assets/image (877).png" alt="Delete" data-size="line"> and a confirmation screen will pop up.

<figure><img src="../../.gitbook/assets/image (878).png" alt="" width="359"><figcaption><p>Deletion Screen</p></figcaption></figure>

To confirm your deletion click on ![Delete](<../../.gitbook/assets/image (976).png>).

{% hint style="danger" %}
_Attention! If you delete an event store, all data related to that event store will be deleted._
{% endhint %}

## Event Streams

Once you create your event stores and pipes, all triggered events will be presented on your Event Streams tab, being available for download according to your data retention settings.

These data will **only** be displayed if there is an event pipe sending data to an event store.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-28 072309.png" alt=""><figcaption><p>Event Streams Tab</p></figcaption></figure>

### Downloading your Event Streams

You are able to download your event streams by clicking on ![](<../../.gitbook/assets/image (864).png>) at the same row as the event stream you want to download. There are two formats of files available:

#### JSON-line

The JSON-line format offers a raw and unfiltered view of the event stream, capturing all relevant information as events occur. This format ensures that no data is left out, giving you complete visibility into each transaction for detailed analysis or integration into custom workflows.

<figure><img src="../../.gitbook/assets/image (865).png" alt=""><figcaption><p>JSON-line</p></figcaption></figure>

Select this format and then click on ![Download](<../../.gitbook/assets/image (978).png>) to download your event stream.

#### CSV

The CSV format provides a customizable and organized view of the event stream, enabling you to choose specific data fields for export. This format makes the data easier to analyze in spreadsheet applications or reporting tools while retaining essential information needed for insights into advertising performance and activity.

<figure><img src="../../.gitbook/assets/image (868).png" alt=""><figcaption><p>CSV</p></figcaption></figure>

It is possible to add or remove columns to your CSV file. To add a column click on <img src="../../.gitbook/assets/image (870).png" alt="" data-size="line">, and then fill in the details:

<figure><img src="../../.gitbook/assets/image (869).png" alt=""><figcaption><p>Add Column</p></figcaption></figure>

* Label - Inform the desired label for the column
* Read Data From - Inform the parameter from where you want to read data
* Default Value - Fill this with a default value for the column, this field is optional.

To remove a column, select it in the list and then click at ![](<../../.gitbook/assets/image (871).png>).

After finishing your settings, click on ![Download](<../../.gitbook/assets/image (978).png>) to download your CSV file.

### Bulk Actions

You can select multiple event streams by checking the <img src="../../.gitbook/assets/image (884).png" alt="Checkbox" data-size="line">, after selecting more than one event, the bulk options will enable, you can download the selected event streams by clicking on <img src="../../.gitbook/assets/image (873).png" alt="" data-size="line">, and selecting one of the file formats available.&#x20;

In order to bulk download event streams you can either select up to 100 individual event streams or select all the event streams.

It's also possible to bulk delete your event streams, click on <img src="../../.gitbook/assets/image (874).png" alt="" data-size="line">, then select delete, and confirm the deletion when it is asked.

### Deleting Event Streams

To delete an event, click on ![](<../../.gitbook/assets/image (889).png>) and a confirmation will be required.

<figure><img src="../../.gitbook/assets/image (890).png" alt="" width="359"><figcaption><p>Event Deletion</p></figcaption></figure>

After clicking on ![Delete](<../../.gitbook/assets/image (976).png>), your event data will be permanently deleted.

{% hint style="danger" %}
_Attention! Be careful when deleting event streams, this action cannot be undone, meaning, your data is permanently removed._
{% endhint %}

## Metrics Tab

Select an event store to visualize the metrics populated by the event pipes, note that you must select an event store to populate when creating an event pipe, if you send your events only to a webhook, the event store will not be populated. These are all the metrics available for the event stores:

* [Stream Bytes](monitoring-metrics.md#stream-bytes)
* [Stream Count](monitoring-metrics.md#stream-count)
* [Stream Upload Bytes](monitoring-metrics.md#stream-upload-bytes)
* [Stream Upload Count](monitoring-metrics.md#stream-upload-count)
* [Stream Download Bytes](monitoring-metrics.md#stream-download-bytes)
* [Stream Download Count](monitoring-metrics.md#stream-download-count)
* [Stream Delete Bytes](monitoring-metrics.md#stream-delete-bytes)
* [Stream Delete Count](monitoring-metrics.md#stream-delete-count)
