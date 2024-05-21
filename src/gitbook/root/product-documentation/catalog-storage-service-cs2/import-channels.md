---
description: Learn more about Import Channels and how to configure them.
---

# Import Channels

Use import channels to upload your products' catalog's feed to our platform, this feature will also keep your catalog updated according to the feed.

## Managing Import Channels

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Import Channels' list</p></figcaption></figure>

### Creating an Import Channel

To start creating an Import Channel, we must first create the catalog which will contain the products imported by the feed, to create a catalog follow the steps in the [Catalogs](catalogs.md) article, we also will need to have a products feed to use as a source for our import channel.

{% hint style="info" %}
_Import Channels can import data from HTTP, FTP or SFTP websites. Google Merchant's XML format is the standard for creating catalogs and the easiest to work with, but the import channel can be configured to use CSV or other XML formats._
{% endhint %}

1. Click on <img src="../../.gitbook/assets/image (10).png" alt="" data-size="line"> to start creating your Import Channel.
2.  Fill in the details on the 3 tabs:\


    <figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption><p>Import Channel editor</p></figcaption></figure>

    1. General Tab
       * Name: Set a name for your Import channel.
       * Tags: Set tags for your organization.
       * Catalog: Select the catalog you've created to receive the products on the feed.
       * When to create or update products: Set the period in which your products will be created or updated.
       * When to remove products:&#x20;
         * Never: Created and updated products at the source will be modified and created in the catalog, however deleting products at the source will not delete these products from the catalog.
         * Before each importation: All products will be deleted from the catalog before each importation and then the products existing on the source will be created in the catalog. The catalog will be empty until the importation's conclusion. All product metrics will be preserved.
         * &#x20;Hours after being imported: Set how long after the importation the products must be deleted from the catalog if not re-imported. As long as the import interval is shorter than the product expiration, the catalog will not be empty. All product metrics are preserved.
    2. Source Tab\

       * Protocol: Select the protocol of your source.
         1.  HTTP:

             <div align="center" data-full-width="false">

             <figure><img src="../../.gitbook/assets/image (110).png" alt=""><figcaption><p>Source Tab - HTTP</p></figcaption></figure>

             </div>

             * URL: Inform your feed's URL
         2.  SFTP and FTP:

             <figure><img src="../../.gitbook/assets/image (112).png" alt=""><figcaption><p>Source Tab - SFTP/FTP</p></figcaption></figure>

             * Host: Inform your source's host.
             * Port: Inform your source's Port.
             * User: Inform a user to access your source.
             * Password: Inform the password to validate your user at the source.
             * Path: Inform the path to your source.
       * Charset: Inform your source's charset.
       * File Format: Select between these options:
         * Google Merchant: Source feed configured using Google Merchant.
         * CSV: Source feed based on a file with comma-separated values.
           * Delimiter: insert the character that separates your file values.
         * XML: Source feed based on an XML file.
           * Item tag: insert the item tag on your XML file.
    3.  Mapping Tab

        * Template: It's necessary to configure the mapping for our system to identify the products' data on your feed, here's an example of mapping:

        <figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption><p>Mapping Tab</p></figcaption></figure>

        * 'offerId': link this field to the column containing your products' IDs.
        * 'title': link this field to the column containing the name of your product.
        * 'description': link this field to the column containing the products' descriptions.
        * 'URL': link this field to the column containing the products' URLs.
        * 'imageUrl': link this field to the column containing the products' image URLs.
        * 'availability': link this field to the column containing data about the products' availability.
        * 'price': link this field to the column containing the products' price.

        _This is only an example of what our mapping can do, there are more fields available, including custom fields. If you need assistance, contact our support team._&#x20;
3. Once you have finished the steps above, check your settings to ensure everything is correct, then click on <img src="../../.gitbook/assets/image (15).png" alt="" data-size="line"> to save your Import Channel.
4.  Click on <img src="../../.gitbook/assets/image.png" alt="" data-size="original"> to start a manual job for importing your products:\


    <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Start Jobs screen</p></figcaption></figure>
5. Click on <img src="../../.gitbook/assets/image (3).png" alt="" data-size="line"> to start importing your products.
6.  It's also possible to import only a few products to test if everything works fine before starting the full import. We can do this by checking the box 'Testing Mode', filling in the details and then clicking on <img src="../../.gitbook/assets/image (4).png" alt="" data-size="line">.\


    <figure><img src="../../.gitbook/assets/image (114).png" alt=""><figcaption><p>Start Jobs screen - Testing Mode</p></figcaption></figure>
7.  Follow your import at the Jobs tab, at this tab we can see the issues with our import or if they were completed. It's possible to understand the problem by clicking on  ![](<../../.gitbook/assets/image (59).png>) or ![](<../../.gitbook/assets/image (60).png>) on the same row as the failed job.\


    <figure><img src="../../.gitbook/assets/image (57).png" alt=""><figcaption><p>Jobs tab</p></figcaption></figure>

### Editing an Import Channel

We can edit our import channels by clicking on <img src="../../.gitbook/assets/image (5).png" alt="" data-size="line"> at the same row that the import channel you need to edit. All details are available for editing.&#x20;

### Deleting an Import Channel

We can delete unused import channels by clicking on <img src="../../.gitbook/assets/image (7).png" alt="" data-size="line"> at the same row that the import channel to be deleted is, however, this will also delete the metrics related to it, so proceed with caution, alternatively we can also archive these import channels by clicking on <img src="../../.gitbook/assets/image (6).png" alt="" data-size="line"> at the same row that the import channel to be archived, to view archived import channels, turn on the option 'Archived' above the import channels' list.
