# Import Channels Metrics

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../../metrics.md).&#x20;
{% endhint %}

The import channels metrics tab contains data about your importing jobs, such as data processing, performance, and failure rate. The metrics tab will display account-wide data for all import channels if no import channel is selected. Selecting a single import channel will show metrics specific to that import channel while selecting multiple import channels will compare their performance.

<figure><img src="../../../.gitbook/assets/image (39) (2).png" alt=""><figcaption><p>Import Channels Metrics Tab</p></figcaption></figure>

### **Import Job Count**

This metric shows how many import jobs you have started in the defined time frame.

<figure><img src="../../../.gitbook/assets/image (279).png" alt=""><figcaption><p>Import Job Count Metric</p></figcaption></figure>

_**Example:** Use this metric to follow how many import jobs are being started on your account**.** On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that there is 1 import job started each day, which means the catalog is being daily updated._

### **Import Job Duration**

This metric shows how much time was taken until the import jobs were concluded in the defined time frame.

<figure><img src="../../../.gitbook/assets/image (280).png" alt=""><figcaption><p>Import Job Duration Metric</p></figcaption></figure>

_**Example:** Use the data obtained on this metric to define the best catalog update option according to your business needs. On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that on June 24th the time until the import job was concluded was nearly 1 second._

### **Import Job Failure Rate**

This metric shows the import job failure rate within the defined time frame, indicating the percentage of import jobs that have failed.

<figure><img src="../../../.gitbook/assets/image (281).png" alt=""><figcaption><p>Import Job Failure Rate Metric</p></figcaption></figure>

_**Example:** When an import job fails, it means that the platform couldn't retrieve any data from the feed file, this could be an issue with the mapping or the source feed file._ _On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that the import job failure rate was 0%, meaning no job has failed._

### **Import Job Issues**

This metric shows the number of issues with import jobs within the defined time frame. Some issues may occur due to invalid or missing data in your feed file. The causes of these issues can be analyzed on the jobs tab.

<figure><img src="../../../.gitbook/assets/image (282).png" alt=""><figcaption><p>Import Job Issues Metric</p></figcaption></figure>

_**Example:** When an import job has been completed, however, some issues occurred on the process, such as a mapping issue or missing data in the feed file**.** On this graph, the defined time frame is 1 week, divided into daily periods, represented as dots. You will notice that during the first 5 days of the week, there were nearly 10 issues with the import job. Additionally, you will observe that on June 24th and onwards, there were no issues with the import job, indicating that the feed file was fixed_

### **Import Job Processed Bytes**

This metric shows the amount of bytes processed during the import jobs in the defined time frame.&#x20;

<figure><img src="../../../.gitbook/assets/image (283).png" alt=""><figcaption><p>Import Job Processed Bytes</p></figcaption></figure>

_**Example:** You can use this to follow the size of the imported feed file on a time frame._ _On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that on each day, almost 1 MB was processed during import jobs._

### **Import Job Processed Records**

This metric shows the amount of records processed during the import jobs in the defined time frame.

<figure><img src="../../../.gitbook/assets/image (284).png" alt=""><figcaption><p>Import Job Processed Records</p></figcaption></figure>

_**Example:** You can use this metric to measure how many records are being processed during your import jobs. On this graph, the defined time frame was 1 week divided into daily periods, represented as dots. You will notice that on the first 5 days, the import job was processing almost 100 records, on the last 2 days, it was processing a little more than 100 records, which means the feed file has been modified._

### Additional Information

These are all the metrics available in the Import Channels feature for analyzing the performance of your import channels. Additionally, when checking metrics, you can always check our <img src="../../../.gitbook/assets/image (28) (2).png" alt="Information" data-size="line"> to access additional information about a specific metric.
