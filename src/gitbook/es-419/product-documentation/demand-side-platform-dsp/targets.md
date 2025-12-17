# Gestión de Objetivos

After creating a Campaign, you will be required to set one Target at least to run the campaign, targets are basically which kind of public you want your campaign to be displayed to, our targets work using **AND** rules not **OR**, so whenever you include a target, you will be restricting your campaign even more to your desired public.

If you set your campaign with broader targets, your budget will be spent more rapidly, since you will be receiving bid requests from a large range of publishers.

## Pre-Targets

These are the targets that will work as the first filter (Location, Cookie Pools, Exchange) and will exclude other possibilities.

Example: If your objective is to target a specific audience from a Cookie Pool, your ads will only be shown to those users inside the Cookie Pool, disregarding other users.

## Targets

You can choose who to show ads to based on where these users are located by either specifying the country and region or by adding geofences around specific addresses.

### **Location**

<figure><img src="../../.gitbook/assets/image (738).png" alt=""><figcaption><p>Location Tab</p></figcaption></figure>

* Geographies - By selecting specific countries or regions, your ads will only appear to users accessing from those geographic locations.
* Geo-fences - By selecting specific countries or regions, your ads will only appear to users accessing from those geographic locations.

### **Contents - Only Websites**

By selecting this target option, your content target will direct your ads only to websites, meaning only website users will receive your ads based on the following content options.

<figure><img src="../../.gitbook/assets/image (97) (1).png" alt=""><figcaption><p>Contents - Only Websites</p></figcaption></figure>

* Languages - By including a particular language, your ads will only appear on websites in that language.
* Categories - By including specific categories, your ads will only appear on websites featuring content in those categories.
* Daily Impressions - Define the minimum number of daily impressions a website must receive to display your ads, ensuring they appear only on sites that meet the required traffic threshold.
* Domains - By including specific domains, your ads will only appear on those specified websites.
* URL Keywords - By defining URL keywords, you can refine where your ads appear based on the URL's content.

### **Contents - Only Apps**

By selecting this target option, your content target will deliver your ads only to apps, meaning that only app users will receive your ads based on the apps' selection.

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption><p>Contents - Only Apps</p></figcaption></figure>

* Apps - By including specific apps, your ads will only appear on those specified apps. Alternatively, excluding certain apps ensures your ads will not be shown on those apps but will remain available on all others. If no app preferences are set, your ads can be displayed on any app, maximizing reach.

{% hint style="info" %}
Please note that we can only display your ads on apps that are connected to one of the Ad Exchanges that we support.
{% endhint %}

### **Contents - Apps and Websites**

By selecting this target option, your content target will deliver your ads to users across both websites and apps. No further segmentation options are available on this tab when this option is selected.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Contents - Apps and Websites</p></figcaption></figure>

* The campaign will target users across both websites and apps, ensuring broad reach. Segmentation options are not available, meaning the campaign will be delivered to all websites and apps without audience filtering. If you wish to specify your targeting, please select either websites only or apps only.

### **Device**

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>

* Operating Systems - By selecting specific operating systems, your ads will be displayed to users navigating the web on those systems.
* Browsers - By selecting specific browsers, your ads will be displayed to users navigating the web through those browsers.
* Device Types - By selecting specific device types, your ads will be displayed to users navigating the web on those devices.
* Cookie Pools - By selecting specific cookie pools, your ads will target only the users who have been added to those selected pools.
* Identifier Pools - By selecting specific identifier pools, your ads will target only the users who have been added to those selected pools.

### **Inventory**

<figure><img src="../../.gitbook/assets/image (839).png" alt=""><figcaption><p>Inventory Tab</p></figcaption></figure>

* Exchange - By selecting specific ad exchanges, your ads will be displayed through those platforms.
* Position - Select specific inventory positions to strategically place your ads for optimal visibility and engagement.
* Viewability - Adjust the slider to set the minimum viewability threshold for ad slots. Your ads will only be matched with inventory positions where the viewability percentage is higher than the selected threshold. This allows for precise control over ad placement, ensuring your ads are only displayed in slots with a visibility level that meets or exceeds your criteria for optimal engagement and impact.
* Click-through rate (CTR) - Adjust the slider to set the minimum Click-Through Rate threshold for ad slots. Your ads will only be matched with inventory where the CTR is higher than the selected threshold. This allows for precise control over ad placement, ensuring your ads are displayed in slots with the CTR level that meets or exceeds your criteria for optimal engagement and impact, the information used for this feature is BMS's database according to all campaigns that are running and collecting data, this feature works for all exchange's inventories.

## Using AI to define Targets

Currently, our platform does not have native AI capabilities. However, feel free to use any AI tool to analyze your data and define your target. Here are a few examples of prompts you can use with your selected AI:

_**Prompt Example 1**: "Based on the provided data, which domains should I focus my campaigns on if my objective is to increase the click-through rate?"_

_**Prompt Example 2**: "Based on the provided data, in which locations will my campaigns be more effective?"_

_**Prompt Example 3**: "Which domains, based on the provided data, should I blacklist to increase my campaigns' click-through rate"_

AI can assist in setting targets that are aligned with your objectives. By analyzing target values, you gain insights for campaign adjustments. For instance, AI can utilize data from our [Monitoring ](../monitoring/)product based on your campaign results and objectives, presenting potential changes for your optimization. For example, when using an [Event Pipe](../monitoring/event-pipes.md) for ADS - Clicked, you can obtain data about which domains are receiving more clicks, allowing you to gain further insights from this information.

## Creating a Target

{% hint style="info" %}
**Before you start**! It's possible to select as many filters as you wish on a single target, however, keep in mind that the difficulty of matching with a publisher will increase as you add more filters, you can also set more than one target with different filters and run your campaign for each one separately.
{% endhint %}

On the selected Campaign page, Press <img src="../../.gitbook/assets/image (49).png" alt="Create Target" data-size="line"> to start creating your target.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (48).png" alt="" width="563"><figcaption><p>Create Target Screen</p></figcaption></figure>

When adding targets, pay attention to the <img src="../../.gitbook/assets/image (385).png" alt="Check" data-size="original"> and <img src="../../.gitbook/assets/image (386).png" alt="Exclude" data-size="line"> signs. These indicate whether you are selecting or excluding a filter for your campaign. The filters you choose will be **listed** in your target filter, showing what will be targeted or excluded from that specific target.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 073343.png" alt=""><figcaption><p>Target Selection or Exclusion</p></figcaption></figure>

After selecting and configuring your target, click on ![](<../../.gitbook/assets/image (676).png>).

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 073834.png" alt=""><figcaption><p>Configured Target Screen</p></figcaption></figure>

You can add as many targets as needed to your campaign, and you can freely turn each target on or off during the campaign to adjust it to your campaign's needs.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Targets List</p></figcaption></figure>

## Estimated Impressions

When creating a target, you will notice that for most of the available target options, there is an estimate of how many impressions can be achieved daily. This estimate represents the median of the daily impressions over the last 7 days.

{% hint style="info" %}
This feature only works with inclusions and is not yet available for URL Keywords.
{% endhint %}

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 075508.png" alt=""><figcaption><p>Estimated Impressions</p></figcaption></figure>

_**Example**: In the picture above, you will notice that for each language, the impressions estimate is shown in the same row as the language. In this example, selecting English and Portuguese will bring you approximately 5.8 million impressions for English and approximately 2.4 million impressions for Portuguese._

Once you select multiple options within a filter, the number of impressions will be summed. After closing the editing group, the total sum will be displayed.

<figure><img src="../../.gitbook/assets/Captura de tela 2025-07-02 112422.png" alt=""><figcaption><p>Estimated Impressions - Total Sum</p></figcaption></figure>

_**Example**: In the picture above, you will notice that English and Portuguese were selected as languages for this target, and their estimated impressions were summed when the group was closed, resulting in a total estimate of 101.5M impressions for both languages combined. Categories and Domains have also been selected. In Categories, you will see that multiple categories were selected, resulting in 165.9M impressions when combined. For Domains, each domain you include adds to the total impressions. In this case, only two domains were selected, resulting in an average of 9.2M impressions._

## Enabling and Disabling a Target

To start a campaign and use your configured target, ensure the targets are enabled if you need to modify or simply stop using a specific target. You can disable it and the campaign will stop using that target immediately.

<figure><img src="../../.gitbook/assets/image (755).png" alt=""><figcaption><p>Target Toggles</p></figcaption></figure>

## Duplicating a Target

If you want to reutilize a dense target but with few changes, you have the option to duplicate that target and save time, simply click on <img src="../../.gitbook/assets/image (123).png" alt="Duplicate Target" data-size="line"> to duplicate your target and a copy of that target will be instantly created.

## Bulk Actions

If you select more than one target, it is possible to make bulk actions.

After selecting two or more targets, the bulk actions button will be enabled, <img src="../../.gitbook/assets/image (753).png" alt="Bulk Actions" data-size="line"> then after clicking on the menu, you will be shown three possibilities which are: **Enable**, **Disable** and **Delete** targets in bulk, this helps you make more actions at once.

## Deleting a Target

If a target is no longer useful for your campaign, you can click on <img src="../../.gitbook/assets/image (124).png" alt="Delete Target" data-size="line"> to permanently delete the target, and a confirmation screen will be shown to you.

<figure><img src="../../.gitbook/assets/image (754).png" alt=""><figcaption><p>Target Deletion</p></figcaption></figure>

{% hint style="danger" %}
_Attention! We always advise disabling the target beforehand and analyzing if it is necessary to delete or simply modify it since the action cannot be undone._
{% endhint %}
