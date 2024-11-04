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

# Catalogs

In the Catalogs tab, you will be able to create a catalog, and then install a pixel to your page so that BMS can collect data from your page based on the following events:

* Product Viewed
* Product Added to Cart
* Product Ordered

By adding those events to your page, we will be able to collect all the data needed to start creating metrics and then use our **Recommendation Models** to improve your ads.

### Creating a Catalog

To create a catalog, click on <img src="../../.gitbook/assets/image (16) (6) (1).png" alt="Create Catalog" data-size="line"> button.

<figure><img src="../../.gitbook/assets/image (17) (6) (1).png" alt="" width="539"><figcaption><p>Create Catalog Screen</p></figcaption></figure>

Choose a **name** for your catalog, and if you wish, add **Tags** to better identify your catalog.

After filling in the fields, click on <img src="../../.gitbook/assets/image (18) (6) (1).png" alt="Save" data-size="line">.

Then your catalog will be available on your list.

<figure><img src="../../.gitbook/assets/image (19) (6) (1).png" alt=""><figcaption><p>Catalog List</p></figcaption></figure>

### Editing a Catalog

If you need to Edit a catalog's name or tags, click on <img src="../../.gitbook/assets/image (20) (4) (1) (1).png" alt="Edit" data-size="line">, after making the necessary changes, click on <img src="../../.gitbook/assets/image (21) (2) (1) (1).png" alt="Save" data-size="line">.

### Archiving a Catalog

To archive a catalog, click on <img src="../../.gitbook/assets/image (22) (2) (1) (1).png" alt="Archive" data-size="line">, then your archived catalog will be shown in the Archived list, to alter your view flip the toggle <img src="../../.gitbook/assets/image (23) (2) (1) (1).png" alt="Toggle" data-size="line">.

### Unarchiving a Catalog

To unarchive a catalog, toggle your view to the Archived list then click on <img src="../../.gitbook/assets/image (24) (2) (1) (1).png" alt="Unarchive" data-size="line">, and your catalog will return to the active catalogs.

### Deleting a Catalog

To delete a catalog, click on <img src="../../.gitbook/assets/image (25) (2) (1).png" alt="Delete" data-size="line">, a screen will be shown to confirm the deletion.

<figure><img src="../../.gitbook/assets/image (26) (2) (1).png" alt=""><figcaption><p>Catalog Deletion Screen</p></figcaption></figure>

After clicking on <img src="../../.gitbook/assets/image (27) (2) (1).png" alt="Delete" data-size="line">, your catalog will be **permanently** deleted.

{% hint style="danger" %}
_Attention! We advise you to deactivate the Catalog instead of completely deleting it. When deleting a Catalog, all data and metrics are lost as well._
{% endhint %}

### How to Track Product Events?

Once you have created your catalog and installed your pixels, and everything is set up correctly, you should start seeing events appear in your metrics. Check our [metrics page](cs2-metrics/) to get a broader view of how events occur and their descriptions.

### Metrics

A broad list of Metrics is available and you can group them by **Catalog**, **Import Channel,** and **Recommendation Model,** each presenting its metrics, should you need any detailed information from a specific metric, hover your cursor over the <img src="../../.gitbook/assets/image (33) (2) (1).png" alt="Information" data-size="line"> and you will have that metric's description.

You can select multiple catalogs for comparison and assess their individual performance.

To have a more broader view on each specific metric go to the [CS2 Metrics](cs2-metrics/#catalog) page.

<figure><img src="../../.gitbook/assets/image (35) (2) (1).png" alt=""><figcaption><p>Catalog Tab Metrics</p></figcaption></figure>

### Install Instructions

In order to activate our metrics and events, you are required to install a pixel on your website to start collecting data.

Select a Catalog where you want to install your pixels and then move to the Install Instructions tab.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Install Instructions Tab</p></figcaption></figure>

Each event has a correct page to have your pixel installed, check on each event description to know exactly where.

Note: Every website has its own way of defining an offerID, so pay attention to how each product is tagged in yours, if you do not use the correct tag for your products, the event **will not work**.

_Example: Product ordered event should be installed on your **order confirmation page**._

