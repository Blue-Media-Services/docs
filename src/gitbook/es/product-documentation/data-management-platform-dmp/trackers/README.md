# Rastreadores

Trackers are small scripts placed on your website's code to gather data on your users' activities, then we can use the collected data to build recommendation models for running retargeting campaigns, improving your conversions. Additionally, this data can provide valuable insights into your users' interests, facilitating the creation of more efficient ad campaigns.

## Managing Trackers

<figure><img src="../../../../es-419/.gitbook/assets/Captura de tela 2024-12-05 074113.png" alt=""><figcaption><p>Trackers list</p></figcaption></figure>

### Creating a Tracker

Trackers will gather data about your website's activities, so it must be installed and active for a while before their data can be used for a campaign.

1. Click on <img src="../../../../es-419/.gitbook/assets/image (92) (1).png" alt="" data-size="line"> to start creating a tracker.
2.  Fill in the details:

    <figure><img src="../../../../es-419/.gitbook/assets/image (1120).png" alt=""><figcaption><p>Tracker Editor</p></figcaption></figure>

    * Name: Set a name for your tracker.
    * Tags: Set tags for your organization.
    * Maximum users: Set the maximum number of users that should be tracked, once the limit is reached, no more new users will be added to the tracker, but the users added will still be tracked.
    * Maximum events per user: Set the maximum number of events per user to keep track, once the limit is reached, receiving new events will cause the oldest ones to be expired.
    * Maximum activity age: Set the number of days for the tracked users' data to be stored, after this period this data will be deleted.
3. Click on <img src="../../../../es-419/.gitbook/assets/image (93) (1).png" alt="" data-size="line"> to save your tracker.

### Editing a Tracker

All the trackers' parameters are editable, click on ![](<../../../../es-419/.gitbook/assets/image (95) (1).png>) in the same row of the tracker you want to edit, make your changes, and then click on ![Save](<../../../../es-419/.gitbook/assets/image (39) (1).png>) to save them.

It's possible to archive trackers for your better organization. Click on ![](<../../../../es-419/.gitbook/assets/image (96) (1).png>) to archive the selected tracker, visualize your archived trackers by turning on the switch "Archived" above the trackers' list. It is also possible to unarchive a tracker by clicking on ![](<../../../../es-419/.gitbook/assets/image (97) (2).png>).

### Deleting a Tracker

We can also delete our trackers by clicking on the delete button ![](<../../../../es-419/.gitbook/assets/image (98) (2).png>) in the same row as the tracker you want to delete and then confirming it by clicking on ![Delete](<../../../../es-419/.gitbook/assets/image (41) (1).png>). This action cannot be undone, so please be careful. Additionally, keep in mind that recommendation models based on the deleted tracker might stop working.

{% hint style="danger" %}
_Attention! Be careful when deleting trackers, this action cannot be undone and all the related data, including previously collected metrics, will also be deleted._
{% endhint %}

## Managing Events and Actions

Configure events to be tracked and actions to be performed by the tracker when the event happens.

<figure><img src="../../../../es-419/.gitbook/assets/image (1).png" alt=""><figcaption><p>Trackers' Configuration Tab</p></figcaption></figure>

### Creating Events and Actions

Configure events according to the activities performed by users on your website, or app, for example adding products to the cart, viewing products, and others.

1. On the Configuration tab, click on <img src="../../../../es-419/.gitbook/assets/image (364).png" alt="" data-size="original"> to start creating an event.
2. Fill in the details:

<figure><img src="../../../../es-419/.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Event Editor</p></figcaption></figure>

* Name: Set a name for your event.
* Event ID: Set an ID for your event, if no ID is set, the Event Name will be used as default event ID.
* Custom Data Fields: Set custom data fields to be collected when the event is captured.
* Currency: Use this field to specify the currency reference for the event. This should reflect the currency in use on your website. It helps track the monetary value associated with the user action.
* Amount: This field captures the quantity associated with the event. For example, in a purchase event, it represents the number of products purchased in a single transaction. Declare a variable on your website that reflects this amount.
* Deduplication ID: This field is used to assign a unique identifier to each event instance. It ensures that duplicated events are not counted multiple times, improving data reliability.
* Template: The template option is available for all fields above. It defines how the values from the event will be processed. It accepts a string using variables from the custom data fields, and generates a comma-separated output.

1. Click on ![](<../../../../es-419/.gitbook/assets/image (364).png>) to add an action to your event, the action is what your tracker will do at BMS once the user access the designed page or perform the specified action.
2. Fill in the details:
   * Name: Set a name for your action.
   *   What to do?:

       <figure><img src="../../../../es-419/.gitbook/assets/Captura de tela 2025-02-27 084243.png" alt=""><figcaption><p>Action Editor</p></figcaption></figure>

       *   Track In Catalog: Allows you to track events based on a product catalog.

           * Catalog: Select the catalog you desire to use.
           * Track as: Select this action as it must be tracked.
           * Field Containing Offer IDs: Select the custom field that contains the offer ID or use a template.
           * Template: Insert a specific template that will be used to create a comma-separated list of offer IDs to be tracked.
           * Available Custom Data: Custom data fields configured on your event will be displayed here to help you build a template.

           <figure><img src="../../../../es-419/.gitbook/assets/Captura de tela 2025-02-27 084528.png" alt=""><figcaption><p>Action Editor</p></figcaption></figure>
       * Track in Identifier Pool: This option allows you to add or remove identifiers from your pools.
         * Identifier Pool: Select the identifier pool you will link to this action.
         * Operation: Select if you want to add or remove identifiers from the pool.
3. Click on <img src="../../../../es-419/.gitbook/assets/image (93) (1).png" alt="" data-size="line"> to save your action.
4. Feel free to add more actions to this event, and when you're done, click on <img src="../../../../es-419/.gitbook/assets/image (93) (1).png" alt="" data-size="line"> to save your event.

### Editing Events and Actions

Edit your events and actions to meet your business needs.

We can edit events by clicking on ![](<../../../../es-419/.gitbook/assets/image (95) (1).png>) at the same row of the event to be edited on the Configuration tab, all events' parameters are available to be edited, after finishing your changes, click on ![Save](<../../../../es-419/.gitbook/assets/image (39) (1).png>) to save them.

Actions' parameters are also editable, you can do this by finding the event that contains the action you want to edit on the Configuration tab, clicking on ![](<../../../../es-419/.gitbook/assets/image (95) (1).png>) at the same row of the event, and then clicking on ![](<../../../../es-419/.gitbook/assets/image (95) (1).png>) at the same row of the action to be edited, make your changes and click on ![Save](<../../../../es-419/.gitbook/assets/image (39) (1).png>) to save your changes, then click on ![Save](<../../../../es-419/.gitbook/assets/image (39) (1).png>) again to save your changes to the event, and you're done.

It's also possible to duplicate events and actions by clicking on ![](<../../../../es-419/.gitbook/assets/image (366).png>) at the same row of the event or action you need to duplicate. This feature can be useful if you need to create a new action or event while keeping some parameters of an existing one.

### Deleting Events and Actions

It's possible to delete events and actions by clicking on ![](<../../../../es-419/.gitbook/assets/image (98) (2).png>) at the same row of the event or action that you need to delete, and then confirm the action by clicking on ![Delete](<../../../../es-419/.gitbook/assets/image (41) (1).png>). This action cannot be undone, so be careful when doing it. Alternatively, it's also possible to disable events and actions by changing the switch position from <img src="../../../../es-419/.gitbook/assets/image (89) (1).png" alt="" data-size="original"> to ![](<../../../../es-419/.gitbook/assets/image (90) (1).png>) in the same row of the event or action you want to disable.

## Install Instructions

After setting up events and actions for your tracker, you have to install it on your website. This can be done by following the instructions on the install instructions tab. Check our [Install Instructions](install-instructions.md) article to learn more about our install methods.

## Metrics Tab

After installing your trackers, you should start receiving data from them. It's possible to follow this process on the metrics tab; these are the available metrics for trackers:

* [Action Execution Count](../dmp-metrics.md#action-execution-count)
* [Action Failure Rate](../dmp-metrics.md#action-failure-rate)
* [Activity Count](../dmp-metrics.md#activity-count)
* [Activity Value](../dmp-metrics.md#activity-value)
* [Expiration Count](../dmp-metrics.md#expiration-count-1)
* [Maximum Users](../dmp-metrics.md#maximum-users)
* [Time Until Expiration](../dmp-metrics.md#time-until-expiration-1)
* [Tracker User Count](../dmp-metrics.md#tracker-user-count)
