# Creatives

Creatives are the smallest building block of our Ad Server. A creative represents what will be delivered to the end user when your ad is displayed.

There are several ways to create or modify creatives. In this page you will learn how to use the Creative list and editor.

Display Creatives are at the end of the day just a block of HTML code. You can provide this code yourself or you can use our built in editor to configure a simple creative that has a clickable image.

All creatives need to be approved by BMS to ensure that it is in accordance with our policies. You can read more about this in the [Review Process](creatives.md#review-process) section.

## Managing Creatives

<figure><img src="../../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption><p>Creative list</p></figcaption></figure>

### Creating a Creative

1. In the Creatives page, click on the <img src="../../.gitbook/assets/create creative.png" alt="Create Creative" data-size="line"> button.
2. Fill in the details:

<figure><img src="../../.gitbook/assets/image (12) (1).png" alt=""><figcaption><p>Creative editor screen</p></figcaption></figure>

* Name - how you want to call this creative;
* Tags - up to 5 labels that can be used to aid identification and searching;
* Domain - this is the primary domain that this creative will take the user when clicked;
* Type - the type of creative, can be any common IAB size like "Large Leaderboard (970x90)", "Banner (468x60)", etc.&#x20;

3. To design your creative you have two options:

* To use a simple image with a link, on the "Static Image" tab, fill:
  * The image you want to display. You can paste an URL for an image you are already hosting or you can use the integration with the BMS Media Library to find or upload a new one.
    * The BMS Media Library supports uploads of static images or GIFs as long as the file size is 2 MB or less.
  * The link you want to open when the image is clicked. You can use any https URL with any query strings such as UTMs. We will add our standard click tracker to be able to show metrics for the creative.
*   To use a fully customized creative, switch to the "Paste HTML" tab and add the final HTML code that will be displayed when the user sees your creative.

    <figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Creative HTML customization tab.</p></figcaption></figure>

    * This can be anything and it is entirely up to you to produce a working creative with HTML, CSS and Javascript.
    * When you provide the HTML code, we will not automatically add our click tracker. You can copy the click tracker macro (or any other macro you wish) from the bottom template assist buttons and paste it on your HTML. Please take a look at the [Macros section](creatives.md#macros) for more information.

4. You can use the <img src="../../.gitbook/assets/preview.png" alt="Preview" data-size="line"> button to check how your creative will be displayed and to make sure that it goes to the correct site when clicking on it.
5. If you are ready to send the creative for review ensure that the "Send for review" option is checked. If you wish to continue editing it later, leave it unchecked.
6. In the end, just hit <img src="../../.gitbook/assets/save.png" alt="Save" data-size="line">.

#### Macros

Our Ad Server provides several macros that can be used within your HTML code. They are:

* BMS Click Tracker - these macros will enable BMS to track clicks on your ads. If you don't install any of these, no click event or metric will be registered.
  * <img src="../../.gitbook/assets/image (17) (1).png" alt="Unescaped Click URL" data-size="line">\
    This is the most used version. It must be installed at the very beginning of the link, before any other tracker and before the final URL itself.
  * <img src="../../.gitbook/assets/image (18) (1).png" alt="Escaped Click URL" data-size="line">\
    This version is similar to the previous but it should only be used if you wish to have an external click tracker that does not support unescaped URLs.
  * <img src="../../.gitbook/assets/image (19) (1).png" alt="Double-escaped Click URL" data-size="line">\
    This version is similar to the previous two but it should only be used if you wish to have a click tracker chain of two or more where the external click tackers do not support unescaped URLs.
* <img src="../../.gitbook/assets/image (20) (1) (1).png" alt="Cache Buster" data-size="line">\
  This macro will inject a random sequence of numbers and is most commonly used to ensure that the requests will not be cached.

### Editing a Creative

To edit a creative use the <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> button on the creative list. All fields are available for editing except the domain and type selectors.

If you modify the image URL, link or the HTML code the creative will go back to the <img src="../../.gitbook/assets/draft status.png" alt="Draft" data-size="line"> status and you will need to send the creative for review again. While in draft the creative will not be shown on any campaigns.

### Enabling and Disabling a Creative

![](<../../.gitbook/assets/image (9) (1) (1) (1) (1).png>)

To be displayed in a campaign a creative must be enabled. If you wish to prevent a creative from being displayed you can disable it and it will immediately cease impressions.

### Archiving and Unarchiving a Creative

Creatives that are not being used as often can be archived by clicking on the <img src="../../.gitbook/assets/archive.png" alt="Archive" data-size="line"> button. Archiving a creative does not prevent it from being used or displayed, just hides it from main view.

To see all archived creatives simply turn on the <img src="../../.gitbook/assets/archive filter.png" alt="Archived" data-size="line"> filter. You can unarchive <img src="../../.gitbook/assets/unarchive.png" alt="Unarchive" data-size="line"> a creative to make it show again on the main list.

### Deleting a Creative

You can delete a creative by clicking on <img src="../../.gitbook/assets/delete.png" alt="Delete" data-size="line">. If the creative is being used, you will be presented with a list of creative groups that will be affected. If you confirm the deletion, the creative groups will be modified to remove the deleted creative from rotation.

<figure><img src="../../.gitbook/assets/image (14) (1).png" alt=""><figcaption><p>Delete confirmation screen showing that the creative is being used.</p></figcaption></figure>

## Review Process

All creatives are reviewed to ensure that they comply with our policies and the policies for our partners.

The review process is usually very quick. If there is any issue it will be displayed as "Rejected" with a tooltip indicating what the reason was. You can make the necessary changes and submit it for review again.

Creatives that pass all validations are marked as <img src="../../.gitbook/assets/approved status.png" alt="Approved" data-size="line">.

A creative will only receive impressions if it is enabled by you and approved by BMS.

## Monitoring Creatives

### Metrics Tab

The metrics tab will display all metrics related to the selected creatives or for the whole account if no creatives are selected.

Learn more about the [metrics tab](../monitoring/metrics.md).

### Real Time Tab

The real time tab will display real time events related to the selected creative.

Learn more about the [real time tab](../campaigns/real-time-tab.md).

