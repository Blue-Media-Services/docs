# Creatives

Creatives are the smallest building block of our Ad Server, representing what will be delivered to the end-user when your ad is displayed.

Display Creatives are essentially just blocks of HTML code. You can provide this code yourself or utilize our built-in editor to configure a simple creative that has a clickable image.

All creatives need to be approved by BMS to ensure compliance with our policies.

## Managing Creatives

<figure><img src="../../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption><p>Creative list</p></figcaption></figure>

### Creating a Creative

To start creating your creative, click on <img src="../../.gitbook/assets/image (2) (1) (1).png" alt="Create Creative" data-size="line">.

Fill in the details:

<figure><img src="../../.gitbook/assets/image (142).png" alt=""><figcaption><p>Creating a Creative</p></figcaption></figure>

* Name - how you want to call this creative;
* Tags - up to 5 labels that can be used to aid identification and searching;
* Domain - the primary domain to which this creative will direct the user when clicked;
* Type - the type of creative, such as common IAB size like "Large Leaderboard (970x90)", "Banner (468x60)", etc.&#x20;

To design your creative, you have two options:

* To use a simple image with a link, on the "Static Image" tab, fill:
  * The image you wish to display. You can either paste an URL for an image you are already hosting or use the integration with the BMS Media Library to find or upload a new one.
    * Note: The BMS Media Library supports uploads of static images or GIFs as long as the file size is 2 MB or less.
  * The link you wish to open when the image is clicked. This can be any HTTPS URL with query strings such as UTMs. Our standard click tracker will be added to show metrics for the creative.
* To use a fully customized creative, switch to the "Paste HTML" tab and insert the final HTML code that will be displayed when the user views your creative.

<figure><img src="../../.gitbook/assets/image (145).png" alt=""><figcaption><p>HTML Code Customization Example</p></figcaption></figure>

* This can be anything and it is entirely up to you to produce a working creative with HTML, CSS, and Javascript.
* When you provide the HTML code, our click tracker won't be automatically added. You can copy the click tracker macro (or any other macro you wish) from the bottom template assist buttons and paste it on your HTML. For more information, please take a look at the [Macros section](creatives.md#macros) .

You can use the <img src="../../.gitbook/assets/preview.png" alt="Preview" data-size="line"> button to see how your creative will be displayed and to make sure that it directs users to the correct site when clicked.

If you are ready to send the creative for review ensure that the "Send for review" option is checked. If you wish to continue editing it later, leave it unchecked.

After making all necessary adjustments, click on ![Save](<../../.gitbook/assets/image (1) (1) (1).png>).

#### Macros

Our Ad Server provides several macros that can be used within your HTML code. They are:

* BMS Click Tracker - these macros will enable BMS to track clicks on your ads. If you don't install any of these, no click event or metric will be registered.
  * <img src="../../.gitbook/assets/image (17) (1).png" alt="Unescaped Click URL" data-size="line">\
    This is the most used version. It must be installed at the very beginning of the link, before any other tracker, and before the final URL itself.
  * <img src="../../.gitbook/assets/image (18) (1).png" alt="Escaped Click URL" data-size="line">\
    This version is similar to the previous but it should only be used if you wish to have an external click tracker that does not support unescaped URLs.
  * <img src="../../.gitbook/assets/image (19) (1).png" alt="Double-escaped Click URL" data-size="line">\
    This version is similar to the previous two but it should only be used if you wish to have a click tracker chain of two or more where the external click tackers do not support unescaped URLs.
* <img src="../../.gitbook/assets/image (20) (1) (1).png" alt="Cache Buster" data-size="line">\
  This macro will inject a random sequence of numbers and is most commonly used to ensure that the requests will not be cached.

### Editing a Creative

To edit a creative use the <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> button on the corresponding creative. All fields are available for editing except the domain and type selectors.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Editing a Creative</p></figcaption></figure>

If you modify the image URL, link or the HTML code the creative will go back to the <img src="../../.gitbook/assets/draft status.png" alt="Draft" data-size="line"> status and you will need to send the creative for review again. While in draft, the creative will not be shown on any campaigns.

Once you have made all necessary changes to your creative, click on ![Save](<../../.gitbook/assets/image (1) (1) (1).png>).

### Enabling and Disabling a Creative

![](<../../.gitbook/assets/image (9) (1) (1) (1) (1).png>)

In order to be displayed in a campaign, a creative must be enabled. If you wish to prevent a creative from being displayed, you can disable it, and it will immediately cease impressions.

### Archiving and Unarchiving a Creative

Creatives that are not being used frequently can be archived by clicking on the <img src="../../.gitbook/assets/archive.png" alt="Archive" data-size="line"> button. Archiving a creative does not prevent it from being used or displayed; it simply hides it from the main view.

To view all archived creatives, simply turn on the <img src="../../.gitbook/assets/archive filter.png" alt="Archived" data-size="line"> filter. You can unarchive <img src="../../.gitbook/assets/unarchive.png" alt="Unarchive" data-size="line"> a creative to return it to the main list.

### Deleting a Creative

You can delete a creative by clicking on <img src="../../.gitbook/assets/delete.png" alt="Delete" data-size="line">. If the creative is being used, you will be presented with a list of creative groups that will be affected. If you confirm the deletion, the creative groups will be modified to remove the deleted creative from the rotation.

<figure><img src="../../.gitbook/assets/image (14) (1).png" alt=""><figcaption><p>Delete confirmation screen showing that the creative is being used.</p></figcaption></figure>

{% hint style="danger" %}
Attention! If you delete a creative, all data related to that creative will also be deleted, this action cannot be undone.
{% endhint %}

## Monitoring Creatives

### Metrics Tab

The metrics tab will display all metrics related to the selected creatives or for the whole account if no creatives are selected.

Learn more about the [Metrics tab](../ad-server/creatives-metrics.md).

### Real Time Tab

The real time tab will display real time events related to the selected creative.

Learn more about the [Real Time tab](../demand-side-platform-dsp/real-time-tab.md).

