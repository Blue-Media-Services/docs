---
description: Learn more about recomendation models and how to create them.
---

# Recommendation Models

Use recommendation models to display your products on dynamic banners, which display different products according to who receives the ad, intending to increase your conversions.

## Managing Recommendation Models

<figure><img src="../../.gitbook/assets/image (62).png" alt=""><figcaption><p>Recommendation Models List</p></figcaption></figure>

### Creating Recommendation Models

Before creating a recommendation model it's necessary to configure catalogs and the DMP services that will act as sources for our recommendation models.

1. Click on <img src="../../.gitbook/assets/image (52).png" alt="" data-size="line"> to start creating a recommendation model.
2.  Fill in the details:\


    <figure><img src="../../.gitbook/assets/image (48) (2).png" alt=""><figcaption><p>Recommendation Models Editor</p></figcaption></figure>

    * Name: Inform a name for your recommendation model.
    * Tags: Set tags for your organization.
    * Catalog: Select the catalog containing the products you will use for this recommendation model.
3. Click on <img src="../../.gitbook/assets/image (53).png" alt="" data-size="line"> to save your recommendation model.

### Configuring Recommendation Models

After creating a recommendation model, it's necessary to configure its sources before being able to use it. This can be done at the configuration tab:

<figure><img src="../../.gitbook/assets/Captura de tela 2024-05-15 095125.png" alt=""><figcaption><p>Recommendation Models Configuration Tab</p></figcaption></figure>

1. Select a recommendation model in the list.
2. Click on <img src="../../.gitbook/assets/image (56).png" alt="" data-size="line"> to add a source for this model.
3.  Fill in the details:\


    <figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption><p>Recommendation Models' Source Editor - DMP Tracker</p></figcaption></figure>

    * Name: Inform a name for your source.
    * Limit: Set the maximum number of products to be added to the recommendation model by this source.
    * Type: Select the type of source you want to use:
      1. DMP Tracker: This option will add products to the recommendation model based on the activity data collected on your website.
         * Tracker: Select the tracker you want to use.
         * Tracker Event: Select the tracked event that will be considered to add products to the recommendation model.
         * Field Containing Offer IDs: Inform the customized field containing the offer ID of the products you want on this recommendation model.
         * Template: Specify a template to produce an offer IDs comma-separated list to track.
      2.  CS2 Product Ranking: This option will add products to the recommendation model based on the activity collected by your product catalog.

          <figure><img src="../../.gitbook/assets/image (51).png" alt=""><figcaption><p>Recommendation Models' Source Editor - CS2 Product Ranking</p></figcaption></figure>

          * Rank by: Select a ranked activity between the options available:
            * Most Added to Cart: This option will add the most added-to-cart products to your recommendation model.
            * Most Ordered: This option will add the most ordered products to your recommendation model.
            * Most Recommendation Clicked: This option can only be used after running a campaign with recommendation models, and it will fill your recommendation model with the products that were recommended before and have been clicked by a user.
            * Most Recommendation Viewed: This option can only be used after running a campaign with recommendation models, and it will fill your recommendation model with the products that were recommended before and have been viewed by a user.
            * Most Recommended: This option can only be used after running a campaign with recommendation models, and it will fill your recommendation model with the most recommended products.
            * Most Viewed: This option will add the most viewed products to your recommendation model
          * In the past hours: Set a number of hours in the past to consider the activity collected during the period for adding products to the recommendation model.
4. Click on <img src="../../.gitbook/assets/image (54).png" alt="" data-size="line"> to save your source.

Right after creating your source, a preview of your recommended products will be available. For this preview to be generated, you should have your cookie pools and trackers and/or your catalog events installed on your website, as their data will be used to generate the recommendations.

<figure><img src="../../.gitbook/assets/image (64).png" alt=""><figcaption><p>Recommendation Models Configuration tab - Preview.</p></figcaption></figure>

### Editing Recommendation Models and Sources

There are some editing options available for recommendation models and sources.

#### Recommendation Models

You can edit a recommendation model's name and tags, however, the catalog cannot be changed. To make this edition click on <img src="../../.gitbook/assets/image (115).png" alt="" data-size="line"> at the same row as the recommendation model to be edited.

#### Sources

All source details are editable, select the recommendation model containing the source to be edited. Then, in the configuration tab, on the sources section, click on <img src="../../.gitbook/assets/image (116).png" alt="" data-size="line"> at the same as the source to be edited, make your changes, then click on <img src="../../.gitbook/assets/image (54).png" alt="" data-size="line"> to save them. You can also duplicate a source by clicking on <img src="../../.gitbook/assets/image (117).png" alt="" data-size="line">. This is useful if you need another source with only a few changes compared to an existing one while keeping the existing one.&#x20;

### How do Sources Work?

Sources are how you collect data to power your Recommendation Model. The Recommendation Model needs this data to organize products as intended. You must choose between a DMP Tracker or a CS2 Product Ranking; both methods work well, but each requires additional steps for proper configuration. Once you have configured your source correctly, your Recommendation Model will start collecting data and actively updating itself, providing your ad with the most current information.

### Deleting Recommendation Models and Sources

{% hint style="danger" %}
Attention! Be careful when deleting recommendation models, this action cannot be undone and all the related data, including previously collected metrics, will also be deleted.
{% endhint %}

You can archive a recommendation model by clicking on <img src="../../.gitbook/assets/image (63).png" alt="" data-size="line"> at the same row as the recommendation model we need archived. It's also possible to delete a recommendation model, however, this will delete all the metrics related to it, this action cannot be undone, so be careful when performing it. Click on <img src="../../.gitbook/assets/image (128).png" alt="" data-size="original"> at the same row as the recommendation model to be deleted. Then confirm the action by clicking on <img src="../../.gitbook/assets/image (129).png" alt="" data-size="line">. This action cannot be undone.&#x20;

It's possible to delete a source. However, this will also delete all the metrics related to this source, so be careful when performing this action. In the sources section of the configuration tab, click on <img src="../../.gitbook/assets/image (128).png" alt="" data-size="original"> at the same row as the source to be deleted. Then confirm the action by clicking on <img src="../../.gitbook/assets/image (129).png" alt="" data-size="line">. This action cannot be undone.

## Metrics Tab

After setting your recommendation models and starting using them for a campaign, you should start receiving data from them, it's possible to follow this process on the metrics tab, these are the available metrics for recommendation models:

* [Product Recommendation Count](cs2-metrics.md#product-recommendation-count)
* [Recommendation Click Count](cs2-metrics.md#recommendation-click-count)
* [Recommendation Fulfillment Rate](cs2-metrics.md#recommendation-fulfillment-rate)
* [Recommendation Request Count](cs2-metrics.md#recommendation-request-count)
* [Recommendation View Count](cs2-metrics.md#recommendation-view-count)
