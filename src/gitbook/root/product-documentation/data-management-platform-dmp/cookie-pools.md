# Cookie Pools

A Cookie Pool is a collection or database of users' cookies. Cookies are tiny pieces of data stored in a user's web browser when they visit a website. These cookies record users' online behavior, preferences, and interactions with websites and services.

In the context of digital advertising and marketing, a cookie pool can serve several purposes:

* **Audience Segmentation:** Segment users into different groups based on their interests, behaviors, demographics, or other criteria. This segmentation allows for more targeted and customized advertising campaigns.
* **Retargeting:** Collect users' data based on events and actions for tracking purposes, this data can be used later to create recommendation models for your retargeting campaigns, improving your conversions. [Learn more about Retargeting campaigns](../../solutions/retargeting.md).
* **Ad Customization:** Use the data gathered to display more relevant ads for each user on your target, based on their recent online activity, interests and behavior, customized ads are more engaging and lead the advertiser to get better results.
* **Analytics and Measurement:** Track your campaigns' performance, measuring click-through rates, conversion rates, user engagement, among other metrics.
* **Frequency Capping:** Set frequency caps to limit how often a particular ad is shown to a user within a certain time frame. This prevents displaying the same ad to the same user repeatedly.

## Managing Cookie Pools

<figure><img src="../../.gitbook/assets/Captura de tela 2025-07-02 095105.png" alt=""><figcaption><p>Cookie Pools list</p></figcaption></figure>

### Creating a Cookie Pool

A cookie pool must be created shortly before using it for a campaign so that it can be populated. Configure how long your cookies should be available before expiring, set how many cookies you want to store at your pool and select the Ad Exchanges you will use to synchronize your cookies with it.

1. Click on ![Create Cookie Pool](<../../.gitbook/assets/image (42).png>) to create a cookie pool.
2.  Fill in the details:\


    <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-15 090606.png" alt=""><figcaption><p>Cookie Pool Editor</p></figcaption></figure>

    * Name: Insert a name for your cookie pool.
    * Tags: Insert tags for your organization.
    * Exchanges: Select ad exchanges to synchronize with your cookies, we recommend selecting only the exchanges you'll use to run your ad campaigns to prevent unnecessary charges.
    * TTL: Set the number of days a cookie will be kept on the pool after syncing.
    * Max Size: Set the maximum amount of cookies that will be stored. After reaching the limit no more cookies will be added to the pool until the old ones expire, but the collected cookies will still be available to use, it's also possible to increase your Max Size to allow more cookies to be collected.
3. Click on ![Save](<../../.gitbook/assets/image (39).png>) to save your Cookie Pool.

### Editing a Cookie Pool

After creating a cookie pool, you can edit it by clicking on the editing button <img src="../../.gitbook/assets/image (7) (1) (1) (1).png" alt="editing button" data-size="line">. All parameters are editable, for the TTL the changes will apply only to newly added cookies. After making your changes, click on ![Save](<../../.gitbook/assets/image (39).png>) to save them.

It's possible to archive cookie pools for your better organization. Click on ![](<../../.gitbook/assets/image (96).png>) to archive the selected cookie pool, visualize your archived cookie pools by turning on the switch "Archived" above the cookie pools list. It is also possible to unarchive a cookie pool by clicking on ![](<../../.gitbook/assets/image (97).png>).

### Deleting a Cookie Pool

{% hint style="danger" %}
Attention! Be careful when deleting cookie pools, this action cannot be undone and all the related data, including previously collected metrics, will also be deleted.
{% endhint %}

You can delete a cookie pool by clicking on the delete button <img src="../../.gitbook/assets/image (8) (1) (1).png" alt="delete button" data-size="original">, a warning that this action cannot be undone will be displayed to you, to proceed with the process click on ![Delete](<../../.gitbook/assets/image (41).png>) to confirm you are deleting it and it's done. Be aware that targets based on these cookie pools will stop working.

## Installing a Cookie Pool

After creating a cookie pool you\`ll need to install it on your website to start using it, this can be done by following the instructions on the Install Instructions tab of the Cookie Pools page.

<figure><img src="../../.gitbook/assets/image (10) (1) (1).png" alt=""><figcaption><p>Install Instructions Tab</p></figcaption></figure>

1. Select the cookie pool you will install by marking the checkbox next to its name.
2. On the Install Instructions tab, click on <img src="../../.gitbook/assets/image (11) (1) (1).png" alt="" data-size="line"> to copy the code.
3. Paste the code as high up as possible inside the page\`s \<head> tag.
4. If you want, it\`s possible to use a unique user id, this is useful if your users log in on multiple devices,  to do this,  uncomment the indicated part of the code and insert the unique user id.

You can also use a tag manager, such as Google Tag Manager (GTM), to add this code to your website.

## Metrics Tab

After installing your cookie pools you should start receiving data from them, it's possible to follow this process on the metrics tab, these are the available metrics for cookie pools:

* [Expiration Count](dmp-metrics.md#expiration-count)
* [Max Size](dmp-metrics.md#max-size)
* [Size](dmp-metrics.md#size)
* [Sync Count](dmp-metrics.md#sync-count)
* [Time Until Expiration](dmp-metrics.md#time-until-expiration)
