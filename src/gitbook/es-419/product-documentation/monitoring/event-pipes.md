# Pipelines de Eventos

Our Event Pipes are used to collect data from all products on our platform. You can use this feature to keep track of everything that can cause an event at BMS, from campaigns to organization creation, allowing you to organize the provided data as you wish.

All event pipes created will be sent to either an Event Store, or you can use a webhook to send this data directly to your data management tool. We provide templates for every event that we can track so you can pick which you want to collect data.

{% hint style="info" %}
We have a solution that may help you understand how a webhook works, check this article [here](../../../es/third-party-integrations/webhook-tool-zapier.md).
{% endhint %}

## Creating an Event Pipe

To create an event store, click on <img src="../../.gitbook/assets/image (276).png" alt="Create Event Pipe" data-size="line"> , and an event pipe creation screen will pop up.

<figure><img src="/broken/files/2SPKQ45kJT8EcGd0p7Yg" alt=""><figcaption><p>Creación de Pipeline de Eventos</p></figcaption></figure>

* Name - Set a name for your Event Store.
* Tags - Create tags to better identify each event pipe.

### Filters

To start configuring your event pipe, pick a template of your choice in our Filters tab according to your needs.

* Sample Event Template - In this dropdown menu, you will be provided with all templates related to the events that we can track.

In this example, we will be creating an event pipe for ADS - Delivered. This event tracks every Ad that is currently running in a campaign and is delivering impressions. Once we create this event pipe, all data will be sent to an Event Store or a Webhook.

<figure><img src="/broken/files/qEMHiii00R8d51np93Ib" alt=""><figcaption><p>ADS - Ad Delivered Pipeline de Eventos</p></figcaption></figure>

Once we have the template selected, you can check which data will be collected when creating the corresponding Event Pipe.

To collect the data, we **must** insert a filter, by clicking on ![Add Filter](<../../.gitbook/assets/image (279).png>).

<figure><img src="/broken/files/xjBUNeQQPD4HUl5rnRfU" alt="" width="515"><figcaption><p>Agregar Filtros</p></figcaption></figure>

* Path - Specific tag in which you can identify the event. Ex: id, type, source, data.accountId.
* Operator - Rule that will be used on this filter.
* Value - The specific value the tag must contain.

In this case, we will be collecting data from ad-delivered events, so this is how the configuration would look.

<figure><img src="../../.gitbook/assets/image (281).png" alt="" width="524"><figcaption><p>Event Pipe Filter Settings</p></figcaption></figure>

We specified the **Path** using the tag "Type", chose the **Operator** option to "Contains" and added the **Value** "Ad-delivered". Note that these fields are case sensitive, so the fulfilled fields **must** match the template.

Once you have fulfilled all fields with the corresponding information based on your event pipe, the test filter must have a check confirming that it is working properly <img src="../../.gitbook/assets/image (282).png" alt="Test Filters Checked" data-size="line">. If it is not working properly due to missing information or a typo, it will be presented with a warning sign <img src="../../.gitbook/assets/image (284).png" alt="Test Filters Warning" data-size="line">.

<figure><img src="../../.gitbook/assets/image (283).png" alt="" width="518"><figcaption><p>Test Filter Warning</p></figcaption></figure>

In this case, our filter failed due to verification in our Value field. These fields are case-sensitive and **must** match the corresponding information.

Once you have added your filters, click on <img src="../../.gitbook/assets/image (979) (1).png" alt="" data-size="line"> to save your event pipe.

### Targets tab

Here you will decide where to send the data: whether it will be sent to one or multiple event stores, a webhook, or a Google Sheet.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 074833.png" alt=""><figcaption><p>Event Pipe's Targets Tab</p></figcaption></figure>

To configure a target, click on ![Add Target](<../../.gitbook/assets/Captura de tela 2024-11-01 083709.png>) and fill out the details according to the chosen target option:

#### Send to Event Store

You must create an event store before using it as a target for your event pipes. Learn more about [Event Stores](event-pipes.md#event-store).

<figure><img src="/broken/files/7c1Qpw1Ep8autQnbL73l" alt=""><figcaption><p>Enviar al Target de Almacén de Eventos</p></figcaption></figure>

If you decide to send your data to an event store, simply name your target and choose your already created event store.

* Name your target.
* Select "Send to Event Store".
* Select the event store you are willing to use.

Once everything is configured, click on <img src="../../.gitbook/assets/image (289).png" alt="Save" data-size="line"> and your event pipe will be listed.

#### Call Webhook

It is possible to send your data to a webhook provided by your data management tool, select this option to use the data management tool of preference, and then fill out the details.

<figure><img src="../../.gitbook/assets/image (980).png" alt=""><figcaption><p>Target de Llamada a Webhook</p></figcaption></figure>

* Name your target.
* Select "Call Webhook".
* Insert your data management tool's webhook URL.

Once you have configured your webhook URL, use our Test Webhook tab to confirm the usability of your webhook tool. Select one of the sample event templates and click on ![Test Webhook](<../../.gitbook/assets/image (981).png>).

If your webhook test is successful, your icon will be presented as ![Test Webhook Successful](<../../.gitbook/assets/image (8) (1).png>) and the tabs for your test will be fulfilled.

* Payload - Information that will be sent to your webhook.
* Result - Status returned and the latency.
* Request - Request used by BMS to send you the information for this test.
* Response - Received response from your webhook.

After finishing all configuration and tests, click on <img src="../../.gitbook/assets/image (979) (1).png" alt="" data-size="line"> to save your target.

#### Google Sheets

You can also send your data to Google Sheets, select this option, and fill out the details.

<figure><img src="/broken/files/plJXtWcXYGHJl0CRfG6I" alt=""><figcaption><p>Target de Google Sheet</p></figcaption></figure>

* Name your target.
* Select "Google Sheets".
* Connect with your Google Account, and you can access the sheet.

Once everything is configured, click on <img src="../../.gitbook/assets/image (289).png" alt="Save" data-size="line"> and your event pipe will be listed.

### Enabling your Event Pipe

To enable an event pipe simply flip the toggle <img src="../../.gitbook/assets/image (510).png" alt="Toggle" data-size="line"> and your event store will be enabled.

<figure><img src="/broken/files/hZitZV2EZGJToYa9887R" alt=""><figcaption><p>Pipeline de Eventos Habilitado</p></figcaption></figure>

### Editing your Event Pipe

To edit your event store, click on <img src="../../.gitbook/assets/image (512).png" alt="Edit" data-size="line"> and an editing screen will pop up, make the necessary changes and then click on <img src="../../.gitbook/assets/image (509).png" alt="Save" data-size="line">.

<figure><img src="/broken/files/FbFcviGACBwh3VdGe0FW" alt="" width="527"><figcaption><p>Pantalla de Edición del Pipeline de Eventos</p></figcaption></figure>

### Bulk Actions

When selecting two or more event pipes, the Bulk Actions will be enabled, allowing you to make actions in bulk.

You will be capable of Archiving and Deleting events in bulk.

<figure><img src="/broken/files/5ueZSQTUA7ufQrxEiLS6" alt=""><figcaption><p>Acciones Masivas del Pipeline de Eventos</p></figcaption></figure>

### Archiving and Unarchiving your Event Pipe

To archive your event pipe, click on <img src="../../.gitbook/assets/image (514).png" alt="Archive" data-size="line"> and it will be sent to the archived list. In order to unarchive your event pipe, switch your view to archived events by flipping the toggle <img src="../../.gitbook/assets/image (515).png" alt="Archived Toggle" data-size="line">. You will then be presented with the list of archived events. Click on <img src="../../.gitbook/assets/image (962) (1).png" alt="Unarchive" data-size="line"> to unarchive an event pipe.

### Deleting your Event Pipe

To delete an event, click on ![](<../../.gitbook/assets/image (975) (1).png>) and a confirmation will be required.

<figure><img src="/broken/files/tSux2ltbMsdt4oKuZtih" alt=""><figcaption><p>Eliminación del Pipeline de Eventos</p></figcaption></figure>

After clicking on <img src="../../.gitbook/assets/image (977) (1).png" alt="Delete" data-size="line">, your event pipe will be deleted.

{% hint style="warning" %}
_We advise users to archive instead of deleting, only delete if you are sure of it, the action cannot be undone._
{% endhint %}

## Metrics Tab

Select an event pipe to access its metrics, selecting more than one will show you a comparison between the selected ones, the metrics are populated once you have created event pipes and they are enabled and collecting data.

These are all the metrics for event pipes:

* [Matched Events Count](../../../es/product-documentation/monitoring/monitoring-metrics.md#matched-events-count)
* [Target Execution Call Count](../../../es/product-documentation/monitoring/monitoring-metrics.md#target-execution-call-count)
* [Target Execution Failure Rate](../../../es/product-documentation/monitoring/monitoring-metrics.md#target-execution-failure-rate)
