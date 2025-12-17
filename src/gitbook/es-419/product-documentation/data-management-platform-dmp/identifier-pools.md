# Pools de Identificadores

Identifier pools function much like cookie pools but are specifically designed for mobile devices, including Android smartphones, tablets, and iOS products. Each operating system employs its own unique methods to identify users effectively.

Google's Android utilizes the GAID (Google Advertising ID), a unique identifier provided by Google Play Services for advertising purposes. The GAID enables developers and advertisers to track user activity and deliver personalized ads, while also giving users control over their privacy settings.

Apple's iOS assigns a unique and random identifier to each user, known as the IDFA (Identifier for Advertisers). Similar to the GAID, the IDFA allows developers and advertisers to monitor user activity and serve tailored ads, all while offering users control over their privacy preferences.

## Managing Identifier Pools

<figure><img src="../../.gitbook/assets/image (470).png" alt=""><figcaption><p>Identifier Pools List</p></figcaption></figure>

### Creating an Identifier Pool

An Identifier Pool must be created before being used for a campaign so that it can be populated. Configure how long the identifiers should be available before expiring, and set how many identifiers you want to store at your pool. Also, select an Ad Exchange to synchronize your Identifiers with it.

1. Click on ![Create Identifier Pool](<../../.gitbook/assets/image (475).png>) to create a new identifier pool.
2.  Fill in the details:

    <figure><img src="../../.gitbook/assets/image (473).png" alt=""><figcaption><p>Identifier Pool Editor</p></figcaption></figure>

    * Name: Inform how you want to name your identifier pool.
    * Tags: Set tags for organizing your identifier pools.
    * Exchanges: Select the desired Ad Exchanges.
    * TTL: Set the number of days you want to keep the identifiers on the pool after added.
    * Max Size: Define how many identifiers can be added to the pool.
3. Click on ![Save](<../../.gitbook/assets/image (476).png>) to save your Identifier Pool.

### Editing an Identifier Pool

After creating an identifier pool, you can edit it by clicking on the editing button ![Edit](<../../.gitbook/assets/image (482).png>). All parameters are editable, for the TTL the changes will apply only to newly added identifiers. After making your changes, click on ![Save](<../../.gitbook/assets/image (476).png>) to save them.

It's possible to archive identifier pools for your better organization. Click on ![Archive](<../../.gitbook/assets/image (1067).png>) to archive the selected identifier pool, and visualize your archived identifier pools by turning on the switch "Archived" above the identifier pools list. It is also possible to unarchive an identifier pool by clicking on ![Unarchive](<../../.gitbook/assets/image (1068).png>).

### Deleting an Identifier Pool

You can delete an identifier pool by clicking on the delete button ![Delete](<../../.gitbook/assets/image (1070).png>), to proceed with the process click on ![Delete](<../../.gitbook/assets/image (1071).png>) to confirm. Be aware that tracker actions based on these identifier pools will stop working.

{% hint style="danger" %}
Attention! Be careful when deleting identifier pools, this action cannot be undone and all the related data, including previously collected metrics, will also be deleted.
{% endhint %}

## Configuring Identifier Pools

After creating an Identifier Pool it is necessary to configure it before using it as a target in a campaign.

To use Identifier Pools you will need to configure a tracker or use an existing one, this article is dedicated to the Identifier Pools feature, access our [Trackers](trackers/) documentation to learn more about configuring a tracker.

### Creating an Action Linked to an Identifier Pool

Follow the steps below in order to create an action for a tracker that will add or remove users to your identifier pools.

After creating and selecting a tracker from the trackers' list, follow the steps below to link it to your identifier pool:

1. On the Configuration tab, in the events tracked section, click on ![Add Event](<../../.gitbook/assets/image (485).png>) to add a new event.
2.  Fill in the details:\\

    <figure><img src="../../.gitbook/assets/image (488).png" alt=""><figcaption><p>Event Editor</p></figcaption></figure>

    * Name: Inform how you want to name this event.
    * Event ID: This field can be customized to set a different event ID, however, it is automatically filled with the event's name.
    * Custom data fields: Set data fields to be collected when the event is captured.
    * Actions: Set actions to be executed when this event is requested, in this article, we will set an action that adds or removes identifiers from our identifiers pool.
      1. Click on ![Add Event](<../../.gitbook/assets/image (485).png>) to add a new action.
      2.  Fill in the details:\\

          <figure><img src="../../.gitbook/assets/Captura de tela 2025-02-27 084528.png" alt=""><figcaption><p>Action Editor</p></figcaption></figure>

          1. Name: Set a name for your event.
          2. Select Track in Identifier Pool
          3. Identifier Pool: Select the identifier pool you will link to this action.
          4. Track as: Select if you want to add or remove identifiers from the pool.
      3. Click on ![Save](<../../.gitbook/assets/image (476).png>) to save your action.
3. Click on ![Save](<../../.gitbook/assets/image (476).png>) again to save your event.

The tracker must be installed on all your website pages where you desire to track user activity, after installing the tracker it might take a while, depending on your website's traffic, until the system gathers identifiers enough for using it as a target in a campaign.

## Metrics Tab

You can follow your Identifier Pools as they grow, this can be done by using the metrics tab of the Identifiers Pool Page. These are all the metrics for this feature:

* [Identifiers Added Count](dmp-metrics.md#identifiers-added-count)
* [Identifiers Enabled Count](dmp-metrics.md#identifiers-enabled-count)
* [Identifiers Expired Count](dmp-metrics.md#identifiers-expired-count)
* [Identifiers Manually Removed Count](dmp-metrics.md#identifiers-manually-removed-count)
* [Max Size](dmp-metrics.md#max-size-1)
* [Size](dmp-metrics.md#size-1)
* [Time Until Expiration](dmp-metrics.md#time-until-expiration-2)
