# DMP Billing

The data management platform billing section details the costs related to this service, divided into up to 6 subsections, depending on the services you have consumed.

<figure><img src="../../.gitbook/assets/image (327).png" alt=""><figcaption><p>DMP Billing</p></figcaption></figure>

{% hint style="info" %}
At BMS, it prioritizes transparency by displaying every detail of your bill. Visit our [Billing Home](../billing.md) to understand how the bills are structured.
{% endhint %}

Below is an explanation of each of these sections with their respective details.

### Cookie Pool Management

In this subsection, you can find information about the costs associated with the cookie pool management service. Deleting items does not incur charges, and for any service within this section, other than stored and configured cookie pools, there is a free quota of 1,000 requests. Once this quota is exceeded, a charge per request will apply. As for stored and configured cookies, charges will be based on the quantity of cookies stored and configured, as well as the duration of storage.

<figure><img src="../../.gitbook/assets/image (329).png" alt=""><figcaption><p>Cookie Pool Management</p></figcaption></figure>

_**Example**: In this picture, you can see that nearly 9,000 cookie-hours were consumed. The charge is not shown as it is less than $0.01. Additionally, almost 825 cookie-pool-hours were consumed, resulting in a $0.86 bill. The free quota on the get cookie pool service was exceeded in 7,120 requests, resulting in a $0.07 bill. Since the other services did not exceed the free quota, no charge was applied to them, totaling a $0.93 bill._

### Cookie Synchronization

This subsection provides details on the cost of the cookie synchronization service. This service is used whenever a cookie in your pool is synchronized with a cookie on the ad exchanges. There is no charge for deletions, and each service includes a free quota of 1,000 requests. Once the free quota is exceeded, a charge per request will be applied.

<figure><img src="../../.gitbook/assets/image (331).png" alt=""><figcaption><p>Cookie Synchronization</p></figcaption></figure>

_**Example**: As observed in this image, none of the listed services have exceeded the free quota, so no charges will be applied._

### Interest Group Management

In this subsection, you will find the cost details for the interest group management service. Deletions are not charged, and there is a free quota of 1,000 requests for each service in this section, except for storage, which will incur charges based on the number of interest groups configured and the duration of storage.

<figure><img src="../../.gitbook/assets/image (332).png" alt=""><figcaption><p>Interest Group Management</p></figcaption></figure>

_**Example**: As observed in this image, none of the listed services have exceeded the free quota, so no charges will be applied._

### Tracker Activity Query

In this subsection, you will find the cost details related to the tracker activity query service. This service is used whenever you request data about your tracker's recent activities. There is a free quota of 1,000 requests for this service; after that, you will be charged per request.

<figure><img src="../../.gitbook/assets/image (326).png" alt=""><figcaption><p>Tracker Activity Query</p></figcaption></figure>

_**Example**: As you can see in this picture, the free quota was not exceeded, and therefore no charges will be applied._

### Tracker Activity Recorder

This subsection details the costs related to the tracker activity recorder service. This service monitors and records your tracker activity. There is a free quota of 1,000 requests for this service; after that, you will be billed per request.

<figure><img src="../../.gitbook/assets/image (333).png" alt=""><figcaption><p>Tracker Activity Recorder</p></figcaption></figure>

_**Example**: In this picture, you can notice that after surpassing the free quota of 1,000 requests, there were nearly 208,000 requests made, resulting in a $2.08 bill._

### Tracker Management

This subsection provides information about the costs associated with the tracker management service. Except for storing configured trackers, all other services in this section come with a free quota of 1,000 requests. Once this quota is exceeded, a charge per request will apply. Deletions do not incur any charges.

<figure><img src="../../.gitbook/assets/image (334).png" alt=""><figcaption><p>Tracker Management</p></figcaption></figure>

_**Example**: In this picture, you will notice that no charge was applied to the services that didn't exceed the free quota, also nearly 1,700 tracker-hours were consumed, resulting in a $0.23 bill._

{% hint style="info" %}
All products generate metrics once you start using them. These metrics are charged and are crucial for understanding your BMS platform usage and performance. The [Monitoring Tab](../monitoring/monitoring-billing.md#metric-monitoring) is responsible for these metrics and will display the related bill.\
BMS is focused on transparency and will show you the costs for all features within each product.
{% endhint %}
