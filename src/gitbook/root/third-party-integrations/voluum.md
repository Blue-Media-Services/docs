---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Voluum

Voluum is a cloud-based analytics platform that helps marketers monitor, optimize, and analyze their digital campaigns. It manages large data volumes and provides real-time insights into key metrics like clicks, conversions, and ROI.

## Tracking BMS Campaigns with Voluum

By integrating BMS with Voluum, advertisers can export campaign data, track specific events, and gain deeper visibility into their campaigns' performance.

<figure><img src="../.gitbook/assets/image (504).png" alt=""><figcaption><p>Voluum Homepage</p></figcaption></figure>

### Tracking Clicks and Impressions

{% hint style="info" %}
This article focuses on integrating **BMS** as a traffic source in **Voluum**. We will not cover Voluum’s full campaign creation options. For more details on Voluum’s features, visit our [**Additional Information**](voluum.md#additional-information) section or [Voluum’s documentation](https://doc.voluum.com/).
{% endhint %}

You must add BMS as a traffic source into your Voluum campaigns to extract data.

1. Select the "Campaigns" tab.
2. Click on "Create" to create a new campaign.
3.  Select "Simple" as creation mode.\


    <figure><img src="../.gitbook/assets/image (505).png" alt=""><figcaption><p>Voluum Campaign Editor - General Tab</p></figcaption></figure>


4. Fill in the details:
   * **General**
     * **Traffic Source**: Search for "BMS" and select it.
     * **Traffic Type**: Select the traffic type based on your campaign's type, Banner, for example.
     * **Country Label**: Select the country where your campaign is running.
     * **Cost Model**: Select the cost model applied to your campaign.
5. After you are satisfied with the remaining parameters, click on Save to proceed.
6.  Select the Tracking and Automizer Tab.\


    <figure><img src="../.gitbook/assets/image (4) (14).png" alt=""><figcaption><p>Voluum Campaign Editor - Tracking &#x26; Automizer Tab</p></figcaption></figure>


7. Here you will find 2 primordial information that will conclude the integration process:
   * **Campaign URL**: This parameter will allow Voluum to track clicks on your BMS campaigns. Use the copy button to copy this link and then use it as your ads link, i.e., paste it into the "Link To" parameter of your ads and creatives.
   * **Impression Click URL**: This parameter will allow Voluum to track impressions on your BMS campaigns. You must copy it using the copy button, paste this URL inside a pixel tag as a source and then add this pixel tag to your creative HTML code.
     * _Example:_ This is an example of a pixel tag:\
       `<img src="VOLUUM_IMPRESSION_PIXEL_URL" style="position: absolute; opacity: 0;">`\
       You must replace the 'src' parameter with the link you copied from Voluum. After replacing it, you will have a result like this:\
       `<img src="https://ImpressionURL.copied/from/Voluum" style="position: absolute; opacity: 0;">`

## Additional Information

After following the steps above, you will start to receive your BMS campaigns' data at Voluum, and the integration will be complete. You can also use the articles below to learn more about our ads creation process and other Voluum features.

* [Creatives](../product-documentation/ad-serving/creatives.md)
* [Ads](../product-documentation/ad-server/ads/)
* [Create a Voluum Campaign](https://doc.voluum.com/article/create-a-voluum-campaign)
* [Add a Traffic Source to Voluum](https://doc.voluum.com/article/add-a-traffic-source-to-voluum)
* [Add an Affiliate Network to Voluum](https://doc.voluum.com/article/add-an-affiliate-network-to-voluum)
