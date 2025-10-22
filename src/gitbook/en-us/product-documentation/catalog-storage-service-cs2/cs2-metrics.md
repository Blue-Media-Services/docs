# CS2 Metrics

These are all the metrics available in the CS2 product for analyzing the performance of your catalogs, products, import channels and recommendation models. Additionally, when reviewing metrics, you can always click the <img src="../../.gitbook/assets/image (462).png" alt="Information" data-size="line"> to access our articles about it.

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../metrics.md).
{% endhint %}

### Product Count

This metric displays the total number of products in your catalog within the specified time frame.

<figure><img src="../../.gitbook/assets/image (458) (3).png" alt=""><figcaption><p>Product Count</p></figcaption></figure>

_**Example**: When importing your catalog's feed it's possible to experience some issues, like a missing product, for example, this metric shows the number of products that are included in your catalog, and this can help you to notice missing products. In this picture, the defined time frame was 8 days, divided into daily periods, you will notice that there are a little more than 1 million products in this catalog, the number of products has changed each day, showing that this catalog is being updated daily._

### Products Added

This metric shows the number of products added to your catalog in the defined time frame.

<figure><img src="../../.gitbook/assets/image (459).png" alt=""><figcaption><p>Products Added</p></figcaption></figure>

_**Example**: You can have your new products added to your catalog anytime you need, this metric will help you to understand how many new products were added to your catalog. In this picture, you can observe that the defined time frame was 8 days, divided into daily periods, on Sep 2, nearly 3 thousand products were added to the catalog, you can also observe that every day, new products were added._

### Products Updated

This metric displays the number of products in your catalog that have been updated in the defined time frame.

<figure><img src="../../.gitbook/assets/image (460).png" alt=""><figcaption><p>Products Updated</p></figcaption></figure>

_**Example**: When updating the catalog, this metric will help you track the number of products that were updated. Use this data to ensure that all the updates made to your feed file were processed by the platform. In this picture, the defined time frame was 8 days divided into daily periods, you will notice that on Sep 2, nearly 3 million products were updated, then, between Sep 3 and Sep 5, almost 4 million products were updated daily, after that we can observe a decreasing number of products updates._

### Products Removed

This metric shows the number of products that were removed from your catalog in the defined time frame.

<figure><img src="../../.gitbook/assets/image (461) (2).png" alt=""><figcaption><p>Products Removed</p></figcaption></figure>

_**Example**: When updating your catalog, this metric will help you track the number of products removed. Use this data to ensure that all the products you removed from the feed file were also removed from your catalog. In this picture, the defined time frame was 9 days divided into daily periods, you will observe that on Sep 9, almost 1 million products were removed from this catalog, and no product was removed between Sep 11 and Sep 15, on Sep 16 a few products were removed from the catalog, and then on Sep 18, we have another huge catalog update, removing almost 1 million products again._

### **Product Added to Cart Count**

This metric shows the number of times the selected products have been added to the cart in the defined time frame.

<figure><img src="../../.gitbook/assets/Product Added to Cart Count (1).png" alt=""><figcaption><p>Product Added to Cart Count Metric</p></figcaption></figure>

_**Example:** In a context where_ &#x79;_&#x6F;u install an event on your website, intending to track products that have been added to the cart by your users. You also configure an action to track the product in the catalog for when this event happens. This metric shows how many times a product has been added to the cart, use this data to understand in which products your website's audience is more interested. This graph's defined time frame was 3 days, divided into 6h periods, represented as dots. You will notice that on June 24th, between 12 PM and 6 PM, nearly 400 products were added to the cart._

### **Product Order Count**

This metric shows the number of times the selected products have been ordered in the defined time frame.

<figure><img src="../../.gitbook/assets/Product Order Count (1).png" alt=""><figcaption><p>Product Order Count Metric</p></figcaption></figure>

_**Example:** In the case where you install an event on your website, intending to track products that your users have ordered. You also configure an action to track the product in the catalog for when this event happens, this metric shows you how many times the selected products have been ordered, use this data to understand in which products your website's audience is more interested. This graph's defined time frame was 3 days, divided into 6h periods, represented as dots. You will notice that on June 24th, between 12 AM and 06 AM, nearly 50 products were ordered._

### **Product View Count**

This metric shows the number of times the selected products were visualized in the defined time frame.

<figure><img src="../../.gitbook/assets/Product View Count (1).png" alt=""><figcaption><p>Product View Count Metric</p></figcaption></figure>

_**Example:** Suppose you have installed on your website a product view event, with an action of track in the catalog, these metrics will show you a count of how many times the selected products were viewed on your website. Use this data to understand which products your audience is more interested in, then create a recommendation model based on this data. This graph's defined time frame was 3 days, divided into 6h periods, represented as dots. You will notice that on June 24th, between 12 AM and 6 AM the selected products were visualized nearly 3000 times._

### **Import Job Count**

This metric shows how many import jobs you have started in the defined time frame.

<figure><img src="../../.gitbook/assets/Import Job Count (1).png" alt=""><figcaption><p>Import Job Count Metric</p></figcaption></figure>

_**Example:** Use this metric to follow how many import jobs are being started on your accoun&#x74;**.** On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that there is 1 import job started each day, which means the catalog is being daily updated._

### **Import Job Duration**

This metric shows how much time was taken until the import jobs were concluded in the defined time frame.

<figure><img src="../../.gitbook/assets/Import Job Duration (1).png" alt=""><figcaption><p>Import Job Duration Metric</p></figcaption></figure>

_**Example:** Use the data obtained on this metric to define the best catalog update option according to your business needs. On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that on June 24th the time until the import job was concluded was nearly 1 second._

### **Import Job Failure Rate**

This metric shows the import job failure rate within the defined time frame, indicating the percentage of import jobs that have failed.

<figure><img src="../../.gitbook/assets/Import Job Failure Rate (1).png" alt=""><figcaption><p>Import Job Failure Rate Metric</p></figcaption></figure>

_**Example:** When an import job fails, it means that the platform couldn't retrieve any data from the feed file, this could be an issue with the mapping or the source feed file._ _On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that the import job failure rate was 0%, meaning no job has failed._

### **Import Job Issues**

This metric shows the number of issues with import jobs within the defined time frame. Some issues may occur due to invalid or missing data in your feed file. The causes of these issues can be analyzed on the jobs tab.

<figure><img src="../../.gitbook/assets/Import Job Issues (1).png" alt=""><figcaption><p>Import Job Issues Metric</p></figcaption></figure>

_**Example:** When an import job has been completed, however, some issues occur in the process, such as a mapping issue or missing data in the feed fil&#x65;**.** On this graph, the defined time frame is 1 week, divided into daily periods, represented as dots. You will notice that during the first 5 days of the week, there were nearly 10 issues with the import job. Additionally, you will observe that on June 24th and onwards, there were no issues with the import job, indicating that the feed file was fixed_

### **Import Job Processed Bytes**

This metric shows the amount of bytes processed during the import jobs in the defined time frame.

<figure><img src="../../.gitbook/assets/Import Job Processed Bytes (1).png" alt=""><figcaption><p>Import Job Processed Bytes</p></figcaption></figure>

_**Example:** You can use this to follow the size of the imported feed file in a time frame._ _On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that on each day, almost 1 MB was processed during import jobs._

### **Import Job Processed Records**

This metric shows the amount of records processed during the import jobs in the defined time frame.

<figure><img src="../../.gitbook/assets/Import Job Processed Records (1).png" alt=""><figcaption><p>Import Job Processed Records</p></figcaption></figure>

_**Example:** You can use this metric to measure how many records are being processed during your import jobs. On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that on the first 5 days, the import job was processing almost 100 records, on the last 2 days, it was processing a little more than 100 records, which means the feed file has been modified._

### **Product Recommendation Count**

This metric shows the number of times the selected products were included in a recommendation in the defined time frame.

<figure><img src="../../.gitbook/assets/Product Recommendation Count (1) (1).png" alt=""><figcaption><p>Product Recommendation Count MetrIc</p></figcaption></figure>

_**Example:** In the context of using a recommendation model for a retargeting campaign, this metric will show you how many times a product was included in a recommendation, use this data to understand which of your products are being recommended on your banners. On this graph, the defined time frame was 1 week divided into 30-minute periods. You will also notice that the product recommendation count was nearly 500 most of the time._

### **Recommendation Click Count**

This metric shows the number of times the selected products' recommendation was clicked in the defined time frame.

<figure><img src="../../.gitbook/assets/Recommendation Click Count (2) (1).png" alt=""><figcaption><p>Recommendation Click Count Metric</p></figcaption></figure>

_**Example:** In case you have a campaign using a recommendation model, this metric will show you a count of clicks on your recommendations, this data will help you to measure your recommendation model efficiency, which will allow you to test different marketing strategies and observe how your audience is reacting on it. On this graph, the defined time frame was 1 week, divided into 6h periods, represented as dots. You will notice that on June 22nd at 12 PM there were 4 clicks on the recommended products._

### **Recommendation Fulfillment Rate**

This metric indicates if the recommendations are being fulfilled with products or if it's missing products in the defined time frame.

<figure><img src="../../.gitbook/assets/Recommendation Fulfillment Rate (1).png" alt=""><figcaption><p>Recommendation Fulfillment Rate Metric</p></figcaption></figure>

_**Example:** Suppose you have a campaign using a recommendation model to generate banners. You will need to set the number of spaces to be filled with recommendations. This metric shows you if your spaces are being fulfilled, use this data to follow if your recommendation models are working properly, which means that the recommendations are being 100% fulfilled, and therefore your banner will not display any empty space. This graph's defined time frame was 1 week, divided into 6h periods, represented as dots. You will notice that on June 24th at 12 AM the recommendation fulfillment rate was nearly 80%, meaning that some spaces on the banner were not filled with products._

### **Recommendation Request Count**

This metric shows the number of times a recommendation was requested in the defined time frame.

<figure><img src="../../.gitbook/assets/Recommendation Request Count (1).png" alt=""><figcaption><p>Recommendation Request Count Metric</p></figcaption></figure>

_**Example:** In case you are using a recommendation model to generate your banners,_ _this metric will show you how many recommendation requests were processed by the platform, this data is useful to follow your consumption of the recommendation models feature. This graph's defined time frame was 1 week, divided into 6h periods, represented as dots. You will notice that on June 23th at 6 PM the recommendation request count was nearly 2000 requests._

### **Recommendation View Count**

This metric shows the number of times the selected product recommendation was viewed in the defined time frame.

<figure><img src="../../.gitbook/assets/Recommendation View Count (1) (1).png" alt=""><figcaption><p>Recommendation View Count Metric</p></figcaption></figure>

_**Example:** In the context where you have a campaign that is using a recommendation model to generate banners, this metric will show you a count of views on your recommendations, the data this metric provides is useful to understand if your recommendations are being viewed, furthermore, comparing this metric with the Recomendation Click Count metric will allow you to understand if your banner is interesting to your targeted audiences._ _On this graph, the defined time frame was 1 week, divided into 6h periods, represented as dots. You will notice that on June 26th at 12 PM there were nearly 4000 views on your recommendations._
