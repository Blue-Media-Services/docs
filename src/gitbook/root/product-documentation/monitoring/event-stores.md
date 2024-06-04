# Event Stores

In our Event Stores tab, you can create a store that acts as a database for storing events. You will be able to create a store where your event pipes will be sent. You can then download the events as a .JSON file and import that to your data management file to better organize it.

<figure><img src="../../.gitbook/assets/image (29).png" alt="" width="563"><figcaption><p>Event Stores Tab</p></figcaption></figure>

## Creating an Event Store

To create an event store, click on <img src="../../.gitbook/assets/image (30).png" alt="Create Event Store" data-size="line"> then an event creation screen will pop up.

<figure><img src="../../.gitbook/assets/image (31).png" alt="" width="361"><figcaption><p>Event Store Creation</p></figcaption></figure>

* Name - Set a name for your Event Store.
* Tags - Create tags to better identify each event store.
* Retention - Decide for how long you will be keeping the data collected by this event store, after expiration, the data will be **deleted**.

After configuring your event store, click on <img src="../../.gitbook/assets/image (32).png" alt="Save" data-size="line"> button to finish your event creation.

### Enabling your Event Store

To enable an event store simply flip the toggle <img src="../../.gitbook/assets/image (33).png" alt="Toggle" data-size="line"> and your event store will be enabled.

<div align="center">

<figure><img src="../../.gitbook/assets/image (34).png" alt="" width="148"><figcaption><p>Event Store Enabled</p></figcaption></figure>

</div>

### Editing your Event Store

To edit your event store, click on <img src="../../.gitbook/assets/image (35).png" alt="Edit" data-size="line"> and an editing screen will pop up, make the necessary changes and then click on <img src="../../.gitbook/assets/image (32).png" alt="Save" data-size="line">.

<figure><img src="../../.gitbook/assets/image (36).png" alt="" width="360"><figcaption><p>Edit Event Store Screen</p></figcaption></figure>

### Bulk Actions

When selecting two or more event stores, the Bulk Actions will be enabled, allowing you to make actions in bulk.

You will be capable of Archiving, Deleting, Enabling and Disabling events in bulk.

<figure><img src="../../.gitbook/assets/image (1) (8).png" alt=""><figcaption><p>Event Stores' Bulk Actions</p></figcaption></figure>

### Archiving and Unarchiving your Event Store

To archive your event store, click on <img src="../../.gitbook/assets/image (37).png" alt="Archive" data-size="line"> and your event store will be sent to the archived list. In order to unarchive your event store, switch your view to archived events by flipping the toggle <img src="../../.gitbook/assets/image (38).png" alt="Archived Toggle" data-size="line">. You will then be presented with the list of archived events. Click on <img src="../../.gitbook/assets/image (39).png" alt="Unarchive" data-size="line"> to unarchive an event store.

### Deleting your Event Store

To delete an event store, click on <img src="../../.gitbook/assets/image (40).png" alt="Delete" data-size="line"> and a confirmation screen will pop up.

<figure><img src="../../.gitbook/assets/image (41).png" alt="" width="359"><figcaption><p>Deletion Screen</p></figcaption></figure>

To confirm your deletion click on <img src="../../.gitbook/assets/image (42).png" alt="Delete" data-size="line">.

{% hint style="danger" %}
_Attention! If you delete an event store, all data related to that event store will be deleted._
{% endhint %}

## Event Streams

Once you create your event stores and pipes, all triggered events will be presented on your Event Streams tab, being available for download according to your data retention settings.

These data will **only** be displayed if there is an event pipe sending data to an event store.

<figure><img src="../../.gitbook/assets/image (132).png" alt=""><figcaption><p>Event Streams Tab</p></figcaption></figure>

### Bulk Actions

You can choose multiple event streams by checking the <img src="../../.gitbook/assets/image (133).png" alt="Checkbox" data-size="line">, after choosing more than one event, you can click on <img src="../../.gitbook/assets/image (135).png" alt="Bulk Actions" data-size="line"> and you will be able to download and delete all checked events.

<figure><img src="../../.gitbook/assets/image (136).png" alt=""><figcaption><p>Bulk Actions Menu</p></figcaption></figure>

### Downloading your Events

To download an event, click on <img src="../../.gitbook/assets/image (137).png" alt="Download" data-size="line"> and your event will be automatically downloaded as a .JSON file, enabling you to send this data to your data management tool.

### Deleting Event Streams

To delete an event, click on ![](<../../.gitbook/assets/image (138).png>) and a confirmation will be required.

<figure><img src="../../.gitbook/assets/image (139).png" alt="" width="359"><figcaption><p>Event Deletion</p></figcaption></figure>

After clicking on <img src="../../.gitbook/assets/image (140).png" alt="Delete" data-size="line">, your event data will be permanently deleted.

{% hint style="danger" %}
_Attention! If you delete an event stream data, it is not possible to restore that data._
{% endhint %}
