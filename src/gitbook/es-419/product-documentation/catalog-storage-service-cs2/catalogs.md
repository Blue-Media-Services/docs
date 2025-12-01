# Catálogos

In the Catalogs tab, you will be able to create a catalog, and then install a pixel to your page so that BMS can collect data from your page based on the following events:

* Product Viewed
* Product Added to Cart
* Product Ordered

By adding those events to your page, we will be able to collect all the data needed to start creating metrics and then use our **Recommendation Models** to improve your ads.

## Managing Catalogs

### Creating a Catalog

To create a catalog, click on <img src="../../.gitbook/assets/image (41).png" alt="Create Catalog" data-size="line"> button.

<figure><img src="../../.gitbook/assets/image (42).png" alt="" width="539"><figcaption><p>Create Catalog Screen</p></figcaption></figure>

Choose a **name** for your catalog, and if you wish, add **Tags** to better identify your catalog.

After filling in the fields, click on <img src="../../.gitbook/assets/image (43).png" alt="Save" data-size="line">.

Then your catalog will be available on your list.

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption><p>Catalog List</p></figcaption></figure>

### Editing a Catalog

If you need to Edit a catalog's name or tags, click on <img src="../../.gitbook/assets/image (45).png" alt="Edit" data-size="line">, after making the necessary changes, click on <img src="../../.gitbook/assets/image (46).png" alt="Save" data-size="line">.

### Archiving a Catalog

To archive a catalog, click on <img src="../../.gitbook/assets/image (47).png" alt="Archive" data-size="line">, then your archived catalog will be shown in the Archived list, to alter your view flip the toggle <img src="../../.gitbook/assets/image (48).png" alt="Toggle" data-size="line">.

### Unarchiving a Catalog

To unarchive a catalog, toggle your view to the Archived list then click on <img src="../../.gitbook/assets/image (49).png" alt="Unarchive" data-size="line">, and your catalog will return to the active catalogs.

### Deleting a Catalog

To delete a catalog, click on <img src="../../.gitbook/assets/image (50).png" alt="Delete" data-size="line">, a screen will be shown to confirm the deletion.

<figure><img src="../../.gitbook/assets/image (51).png" alt=""><figcaption><p>Catalog Deletion Screen</p></figcaption></figure>

After clicking on <img src="../../.gitbook/assets/image (52).png" alt="Delete" data-size="line">, your catalog will be **permanently** deleted.

{% hint style="danger" %}
_Attention! We advise you to deactivate the Catalog instead of completely deleting it. When deleting a Catalog, all data and metrics are lost as well._
{% endhint %}

## Installing Catalogs

In order to activate our metrics and events, you are required to install a pixel on your website to start collecting data.

Select a Catalog where you want to install your pixels and then move to the Install Instructions tab.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Install Instructions Tab</p></figcaption></figure>

Each event has a correct page to have your pixel installed, check on each event description to know exactly where.

{% hint style="info" %}
Remember to replace the placeholder with your offer ID. Every website has its own way of defining an offer ID variable, so pay attention to how this variable was configured in your website. If the correct variable is not used for your products, the event **will not work.** Ensure that the offer ID variable on your website returns the same values that were imported as product identifiers (on our platform, they are called Offer IDs) in your catalog.
{% endhint %}

_**Example:** The Product ordered event should be installed on your **order confirmation page**._

## Metrics Tab <a href="#metrics" id="metrics"></a>

Once you have created your catalog and correctly installed your pixels, the metrics will begin to be populated and you will be able to track the events as they happen.

A broad list of Metrics is available and it is possible to group them by **Catalog**, **Import Channel,** and **Recommendation Model,** each presenting its metrics. You can also select multiple catalogs for comparison and assess their performance.

These are all the metrics available for the Catalogs feature:

* [Import Job Count](cs2-metrics.md#import-job-count)
* [Import Job Duration](cs2-metrics.md#import-job-duration)
* [Import Job Failure Rate](cs2-metrics.md#import-job-failure-rate)
* [Import Job Issues](cs2-metrics.md#import-job-issues)
* [Import Job Processed Bytes](cs2-metrics.md#import-job-processed-bytes)
* [Import Job Processed Records](cs2-metrics.md#import-job-processed-records)
* [Product Added To Cart Count](cs2-metrics.md#product-added-to-cart-count)
* [Product Count](cs2-metrics.md#product-count)
* [Product Order Count](cs2-metrics.md#product-order-count)
* [Product Recommendation Count](cs2-metrics.md#product-recommendation-count)
* [Product View Count](cs2-metrics.md#product-view-count)
* [Products Added](cs2-metrics.md#products-added)
* [Products Removed](cs2-metrics.md#products-removed)
* [Products Updated](cs2-metrics.md#products-updated)
* [Recommendation Click Count](cs2-metrics.md#recommendation-click-count)
* [Recommendation Fulfillment Rate](cs2-metrics.md#recommendation-fulfillment-rate)
* [Recommendation View Count](cs2-metrics.md#recommendation-view-count)
* [Recommendation Request Count](cs2-metrics.md#recommendation-request-count)
