# Managing Targets

After creating a Campaign, you will be required to set one Target at least to run the campaign, targets are basically which kind of public you want your campaign to be displayed to, our targets work using **AND** rules not **OR**, so whenever you include a target, you will be restricting your campaign even more to your desired public.

If you set your campaign with broader targets, your budget will be spent more rapidly, since you will be receiving bid requests from a large range of publishers.

### Pre-Targets

These are the targets that will work as the first filter (Location, Cookie Pools, Exchange) and will exclude other possibilities.&#x20;

Example: If your objective is to target a specific audience from a Cookie Pool, your ads will only be shown to those users inside the Cookie Pool, disregarding other users.

### Targets

You can choose who to show ads to based on where these users are located by either specifying the country and region or by adding geofences around specific addresses.

<figure><img src="../../.gitbook/assets/image (337).png" alt=""><figcaption><p>Location Tab</p></figcaption></figure>

* **Location**
  * Geographies - By selecting specific countries or regions, your ads will only appear to users accessing from those geographic locations.
  * Geo-fences - By selecting specific countries or regions, your ads will only appear to users accessing from those geographic locations.

<figure><img src="../../.gitbook/assets/image (338).png" alt=""><figcaption><p>Contents Tab</p></figcaption></figure>

* **Contents**
  * Languages - By including a particular language, your ads will only appear on websites in that language.
  * Categories - By including specific categories, your ads will only appear on websites featuring content in those categories.
  * Domains - By including specific domains, your ads will only appear on those specified websites.
  * URL Keywords - By defining URL keywords, you can refine where your ads appear based on the URL's content.

<figure><img src="../../.gitbook/assets/image (339).png" alt=""><figcaption><p>Device Tab</p></figcaption></figure>

* **Device**
  * Operational Systems - By selecting specific operating systems, your ads will be displayed to users navigating the web on those systems.
  * Browsers - By selecting specific browsers, your ads will be displayed to users navigating the web through those browsers.
  * Device Types - By selecting specific device types, your ads will be displayed to users navigating the web on those devices.
  * Cookie Pools - By selecting specific cookie pools, your ads will target only the users who have been added to those selected pools.

<figure><img src="../../.gitbook/assets/image (340).png" alt=""><figcaption><p>Inventory Tab</p></figcaption></figure>

* **Inventory**
  * Exchange - By selecting specific ad exchanges, your ads will be displayed through those platforms.
  * Position - Select specific inventory positions to strategically place your ads for optimal visibility and engagement.
  * \*Viewability - Adjust the slider to set the minimum viewability threshold for ad slots. Your ads will only be matched with inventory positions where the viewability percentage is higher than the selected threshold. This allows for precise control over ad placement, ensuring your ads are only displayed in slots with a visibility level that meets or exceeds your criteria for optimal engagement and impact. \
    \*This target option is in beta and currently is only supported by Google Authorized Buyers.

### Using AI to define Targets

AI can assist in setting targets aligned with your objectives. By analyzing target values, you gain insights for campaign adjustments. For instance, AI utilizes data from our [Monitoring ](../monitoring/)product based on your campaign results and objectives. The AI will present potential changes for your campaign. For example, when using an [Event Pipe](../monitoring/event-pipes.md) for ADS - Clicked, you can obtain data related to which domains are being clicked on more often. Additionally, you might gain further insights from this information.

You can use any AI you desire to analyze your data and help you define your target.

### Creating a Target

In the selected Campaign page, Press <img src="../../.gitbook/assets/image (3) (3).png" alt="Create Target" data-size="line">to start creating your target.

<figure><img src="../../.gitbook/assets/image (242).png" alt="" width="434"><figcaption><p>Targets List</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2) (3).png" alt="" width="563"><figcaption><p>Create Target Screen</p></figcaption></figure>

When adding targets, pay attention to the <img src="../../.gitbook/assets/image (84).png" alt="Check" data-size="original"> and <img src="../../.gitbook/assets/image (85).png" alt="Exclude" data-size="line"> signs. These indicate whether you are selecting or excluding a filter for your campaign. The filters you choose will be **listed** in your target filter, showing what will be targeted or excluded from that specific target.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 073343.png" alt=""><figcaption><p>Target Selection or Exclusion</p></figcaption></figure>

After selecting and configuring your target, click on ![](<../../.gitbook/assets/image (253).png>).

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 073834.png" alt=""><figcaption><p>Configured Target Screen</p></figcaption></figure>

You can add as many targets as needed to your campaign, and you can freely turn each target on or off during the campaign to adjust it to your campaign's needs.

<figure><img src="../../.gitbook/assets/image (243).png" alt="" width="434"><figcaption><p>Targets List</p></figcaption></figure>

### Estimated Impressions

{% hint style="info" %}
This feature only works with inclusions and is not yet available for Geofences, URL Keywords, and Categories.
{% endhint %}

When creating a target, you will notice that for most of the available target options, there is an estimate of how many impressions can be achieved daily. This estimate represents the median of the daily impressions over the last 7 days.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 075508.png" alt=""><figcaption><p>Estimated Impressions</p></figcaption></figure>

_**Example**: In the picture above, you will notice that for each language, the impressions estimate is shown in the same row as the language. In this example, selecting English and Portuguese will bring you approximately 5.8 million impressions for English and approximately 2.4 million impressions for Portuguese._

Once you select multiple options within a filter, the number of impressions will be summed. After closing the editing group, the total sum will be displayed.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Estimated Impressions - Total Sum</p></figcaption></figure>

_**Example**: In the picture above, you will notice that English and Portuguese were selected as languages for this target, and their number of estimated impressions was summed when the group was closed, resulting in a total estimate of 8.2M impressions for both languages combined._

### Enabling and Disabling a Target

To start a campaign and use your configured target, ensure the targets are enabled. If you need to modify or simply stop using a specific target. You can disable it and the campaign will stop using that target immediately.

<figure><img src="../../.gitbook/assets/image (246).png" alt=""><figcaption><p>Target Toggles</p></figcaption></figure>

### Duplicating a Target

If you want to reutilize a dense target but with few changes, you have the option to duplicate that target and save time, simply click on <img src="../../.gitbook/assets/image (42) (1).png" alt="Duplicate Target" data-size="line"> to duplicate your target and a copy of that target will be instantly created.

### Deleting a Target

If a target is no longer useful for your campaign, you can click on <img src="../../.gitbook/assets/image (43) (1).png" alt="Delete Target" data-size="line"> to permanently delete the target, and a confirmation screen will be shown to you.&#x20;

<figure><img src="../../.gitbook/assets/image (245).png" alt=""><figcaption><p>Target Deletion</p></figcaption></figure>

{% hint style="danger" %}
_Attention! We always advise disabling the target beforehand and analyzing if it is necessary to delete or simply modify it since the action cannot be undone._
{% endhint %}

### Bulk Actions

If you select more than one target, it is possible to make bulk actions.

After selecting two or more targets, the bulk actions button will be enabled, <img src="../../.gitbook/assets/image (244).png" alt="Bulk Actions" data-size="line"> then after clicking on the menu, you will be shown three possibilities which are: **Enable**, **Disable** and **Delete** targets in bulk, this helps you make more actions at once.
