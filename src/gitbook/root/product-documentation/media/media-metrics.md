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

# Media Metrics

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../metrics.md).
{% endhint %}

Once you populate your account with media for creating creatives, our platform will begin providing metrics related to all the media stored in your account.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-10 081603.png" alt=""><figcaption><p>Media Metrics</p></figcaption></figure>

### **Media Count**

This metric represents the total count of media stored by the user during the selected time period. It updates hourly and accumulates over a 24h period.

<figure><img src="../../.gitbook/assets/Media Count.png" alt=""><figcaption><p>Media Count Metric</p></figcaption></figure>

_**Example:** This metric shows an increase in the amount of media in the library at some point in May. Later, some of that media was removed because it was no longer being used. It reached a peak of 2,000 media files and ended with nearly 500. It is important to note that BMS charges per media file and media size stored on the platform, so performing a cleanup from time to time might be useful._

### **Media Download Count**

This metric is populated by each media that has been displayed on a domain, after successfully winning an auction, the media will be downloaded to the end user's browser.

<figure><img src="../../.gitbook/assets/Media Download Count.png" alt=""><figcaption><p>Media Download Count</p></figcaption></figure>

_**Example**: If your creative has been created using media from BMS's Library, our platform can identify that the media has been downloaded in the end user's browser after winning the bidding. Then, the metric is populated, informing the performance of the media. In this graph, you can see that a peak of nearly 55,000 downloads was reached._

### **Media Downloaded Bytes**

This metric represents the total bytes used upon media downloaded to the end user's browser, this metric will follow the same parameters as the download count if no creative size is changed.

<figure><img src="../../.gitbook/assets/Media Downloaded Bytes.png" alt=""><figcaption><p>Media Downloaded Bytes</p></figcaption></figure>

_**Example**: On this graph,you can see that the size of media downloaded peaked at nearly 6 to 7 GB. It is beneficial to work with this information to try reducing the size of your media, making it faster to be downloaded in the end user's browser, ensuring your ad will be shown._

### **Media Stored Bytes**

This metric represents the total bytes of your media stored on BMS, size may vary according to the currently stored media.

<figure><img src="../../.gitbook/assets/Media Stored Bytes.png" alt=""><figcaption><p>Media Stored Bytes Metric</p></figcaption></figure>

_**Example**: According to this metric, the size peaked at nearly 400 MB. However, after removing a few media files, it stabilized at around 200 MB and decreased further following another cleanup of the media library. Since the platform charges per byte stored in the library, it might be beneficial to perform cleanups from time to time, as well as check if any optimization is possible for your media's size._

### **Media Upload Count**

This metric represents the total media uploaded during the selected time period. It updates each time you add media to your library.

<figure><img src="../../.gitbook/assets/Media Upload Count.png" alt=""><figcaption><p>Media Upload Count Metric</p></figcaption></figure>

_**Example**: This metric shows that media were added to the library daily, reaching a peak of nearly 35 uploads in a single day. The number of uploads decreased afterward due to fewer media being added, this helps you keep track of how much of the library are you currently using to store your media._

### **Media Uploaded Bytes**

This metric represents the total amount of data, in bytes, for your uploaded media. It helps you track how much storage you are using on BMS for each uploaded media file.

<figure><img src="../../.gitbook/assets/Media Uploaded Bytes.png" alt=""><figcaption><p>Media Uploaded Bytes Metric</p></figcaption></figure>

_**Example**: Between May and June, there was a peak of 4 MB in uploads on a single day. This metric may differ from the Media Upload Count metric because each file varies in size, leading to minor differences, such as those observed during the transition from April to May. It is important to note that the size of a media file impacts how long the end user takes to download it on their browser._

### Additional Information

These are all the metrics available in the Media product for analyzing the storage of your media.  Additionally, when checking metrics, you can always check our <img src="../../.gitbook/assets/image (28) (2).png" alt="Information" data-size="line"> to access additional information about a specific metric.
