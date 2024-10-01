# Import Channels

Use import channels to upload your products' catalog's feed to our platform, this feature will also keep your catalog updated according to the feed.

## Managing Import Channels

<figure><img src="../../.gitbook/assets/image (8) (6) (1).png" alt=""><figcaption><p>Import Channels' list</p></figcaption></figure>

### Creating an Import Channel

To start creating an Import Channel, we must first create the catalog which will contain the products imported by the feed, to create a catalog follow the steps in the [Catalogs](catalogs.md) article, we also will need to have a products feed to use as a source for our import channel.

{% hint style="info" %}
_Import Channels can import data from HTTP, FTP or SFTP websites. Google Merchant's XML format is the standard for creating catalogs and the easiest to work with, but the import channel can be configured to use CSV or other XML formats._
{% endhint %}

1. Click on <img src="../../.gitbook/assets/image (10) (6) (1).png" alt="" data-size="line"> to start creating your Import Channel.
2.  Fill in the details on the 3 tabs:\


    <figure><img src="../../.gitbook/assets/image (13) (6) (1).png" alt=""><figcaption><p>Import Channel editor</p></figcaption></figure>

    1. General Tab\
       On this tab, you will find the general details related to your import channel, use the examples to help you fill in all the details.
       * Name: Set a name for your Import channel.
       * Tags: Set tags for your organization.
       * Catalog: Select the catalog you've created to receive the products on the feed.
       * When to create or update products: Set the period in which your products will be created or updated.
       * When to remove products:&#x20;
         * Never: Created and updated products at the source will be modified and created in the catalog, however deleting products at the source will not delete these products from the catalog.
         * Before each importation: All products will be deleted from the catalog before each importation and then the products existing on the source will be created in the catalog. Beware! The catalog will be empty until the importation's conclusion, so the ad banners generated during this period might be empty. All product metrics will be preserved.
         * &#x20;Hours after being imported: Set how long after the importation the products must be deleted from the catalog if not re-imported. As long as the import interval is shorter than the product expiration, the catalog will not be empty. All product metrics are preserved.
    2.  Source Tab\
        This tab contains the source details related to your import channel, use the examples to help you fill in these details according to your source option.

        * Protocol: Select the protocol of your source and fill the details according to your choice.
          1.  HTTP:

              <div align="center" data-full-width="false">

              <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-27 121710.png" alt=""><figcaption><p>Source Tab - HTTP</p></figcaption></figure>

              </div>

              * URL: Inform your feed's URL
          2.  SFTP and FTP:

              <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-22 090041.png" alt=""><figcaption><p>Source Tab - SFTP/FTP</p></figcaption></figure>

              * Host: Inform your source's host.
              * Port: Inform your source's Port.
              * User: Inform a user to access your source.
              * Password: Inform the password to validate your user at the source.
              * Path: Inform the path to your source.
        * Test Source: This button, <img src="../../.gitbook/assets/image (356).png" alt="" data-size="line">, allows you to test your source and retrieve relevant data for the next fields. There are three tabs for the source test result:
          * Detected Records: Display your feed's records in table format.
          * Issues: Display the problems that can affect your import job.
          *   Raw: Display your feed file source code.\


              <figure><img src="../../.gitbook/assets/image (355).png" alt=""><figcaption><p>Source Test Result</p></figcaption></figure>

        After finishing the test click on <img src="../../.gitbook/assets/image (357).png" alt="" data-size="line"> to close the source test result window and automatically fill the next fields with your test results.

        * Charset: Inform the source's charset, which was previously detected on the source test result.
        * File Format: The source test result will automatically fill these fields, however, you can change them manually.  Select between these options:
          * CSV: Source feed based on a file with comma-separated values.
            * Delimiter: insert the character that separates your file values.
          * XML: Source feed based on an XML file.
            * Item tag: insert the item tag on your XML file.
    3.  Mapping Tab\
        You will find on this tab the mapping details related to your import channel, use the examples to help you to configure your mapping.

        *   Template Format: Select between these two options:

            * Google Shopping: Select this option if you are using a Google Shopping Feed.

            <figure><img src="../../.gitbook/assets/image (352) (1).png" alt=""><figcaption><p>Mapping Tab - Google Shopping</p></figcaption></figure>

            * Advanced: For any other kind of feed file, select this option.

            <figure><img src="../../.gitbook/assets/image (354).png" alt=""><figcaption><p>Mapping Tab - Advanced</p></figcaption></figure>
        * Detect Template: Click on <img src="../../.gitbook/assets/image (359).png" alt="" data-size="line"> to detect the best template based on your feed file.
        * Test Template: Click on <img src="../../.gitbook/assets/image (362).png" alt="" data-size="line"> to access a preview of how your products will be displayed in your catalog. If there are any failures with the mapping or the feed file, you will notice them on this test.

        <figure><img src="../../.gitbook/assets/Captura de tela 2024-09-18 145710.png" alt=""><figcaption><p>Mapping Test Result</p></figcaption></figure>

        * Click on <img src="../../.gitbook/assets/image (364).png" alt="" data-size="line"> to proceed.
3. Once you have finished the steps above, check your settings to ensure everything is correct, then click on <img src="../../.gitbook/assets/image (15) (6) (1).png" alt="" data-size="line"> to save your Import Channel.
4.  Click on <img src="../../.gitbook/assets/image (2) (1) (2) (1).png" alt="" data-size="original"> to start a manual job for importing your products:\


    <figure><img src="../../.gitbook/assets/image (2) (1) (2) (1) (1).png" alt=""><figcaption><p>Start Jobs screen</p></figcaption></figure>
5. Click on <img src="../../.gitbook/assets/image (3) (6).png" alt="" data-size="line"> to start importing your products.
6.  It's also possible to import only a few products to test if everything works fine before starting the full import. We can do this by checking the box 'Testing Mode', filling in the details and then clicking on <img src="../../.gitbook/assets/image (4) (6) (1).png" alt="" data-size="line">.\


    <figure><img src="../../.gitbook/assets/image (114).png" alt=""><figcaption><p>Start Jobs screen - Testing Mode</p></figcaption></figure>
7.  Follow your import at the Jobs tab, at this tab we can see the issues with our import or if they were completed. It's possible to understand the problem by clicking on  ![](<../../.gitbook/assets/image (59).png>) or ![](<../../.gitbook/assets/image (60).png>) on the same row as the failed job.\


    <figure><img src="../../.gitbook/assets/image (57).png" alt=""><figcaption><p>Jobs tab</p></figcaption></figure>

### Editing an Import Channel

We can edit our import channels by clicking on <img src="../../.gitbook/assets/image (5) (6) (1).png" alt="" data-size="line"> at the same row that the import channel you need to edit. All details are available for editing.&#x20;

### Deleting an Import Channel

We can delete unused import channels by clicking on <img src="../../.gitbook/assets/image (7) (6) (1).png" alt="" data-size="line"> at the same row that the import channel to be deleted is, however, this will also delete the metrics related to it, so proceed with caution, alternatively we can also archive these import channels by clicking on <img src="../../.gitbook/assets/image (6) (6) (1).png" alt="" data-size="line"> at the same row that the import channel to be archived, to view archived import channels, turn on the option 'Archived' above the import channels' list.
