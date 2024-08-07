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

# Ad Serving Billing

The ad serving billing section is available on the billing page. It contains information about every billed item related to ad serving and is divided into 9 sub-sections.

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption><p>Ad Serving Billing Section</p></figcaption></figure>

{% hint style="info" %}
At BMS, it prioritizes transparency by displaying every detail of your bill. Visit our [Billing Home](../billing.md) to understand how the bills are structured.
{% endhint %}

Below is an explanation of each of these sections with their respective details.

### Ad Management

The ad management subsection details the costs associated with the ad management process. Storing ads incurs a fee based on the duration of storage and the number of ads stored. Additionally, there is a complimentary quota of 1,000 requests for each of the following services: ad creation, ad requests, ad patching, and ad listing. Charges apply once this free quota is exceeded. Deleting actions are not charged.

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption><p>Ad Management</p></figcaption></figure>

_**Example**:_ _In the picture, there were almost 63 thousand ad hours consumed, which is equivalent to keeping nearly 88 ads active for a month (720 hours). This results in a bill of $8.80. Additionally, there were nearly 73 thousand ad requests; the first thousand were free, and after that, the ad requests were billed at $0.01 per thousand, resulting in a $0.73 bill. Therefore, the total Ad Management bill ($8.80 + $0.73) was $9.52._

### Ad Rendering

The ad rendering subsection details the costs related to the ad rendering service. You will be charged per request when retrieving an ad container or ad content. Additionally, the charges for rendering an ad will be based on the number of ad content bytes transferred during the process.

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption><p>Ad Rendering</p></figcaption></figure>

_**Example**: You will notice that in this picture there were nearly 103 thousand ad content requests. The charge was $0.10 per 1,000 ad content requests, resulting in a $10.27 bill. It is also possible to notice that 0.57 GB of ad content data was transferred. The charge was $1.00 per GB transferred, costing $0.57 for the ad content data transferred. Since the ad container only has 56 requests and is charged $0.01 per 1,000 requests, it did not contribute to the final result, meaning the total Ad Rendering bill ($10.27 + $0.57) was $10.84._

### Ad Tracking

This subsection outlines the costs associated with the ad tracking service. Each service in this section includes a free quota of 1,000 requests. You will only incur charges once this quota is exceeded. Fees are based on the number of requests processed during your ad campaign.

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption><p>Ad Tracking</p></figcaption></figure>

_**Example**: In the image, you can observe that there was a free quota of 1,000 requests per service, after which billing starts. It is noticeable that this quota was not reached for the Ad Click Tracking service, meaning there will be no charges for this service. You can also observe that after reaching the quota, the Ad Display Tracking service is charged $0.001 per 1,000 requests. There were nearly 93 thousand requests for this service, resulting in a $0.09 bill. Additionally, after the Track Ad View passed the 1,000 requests mark, it charged for nearly 48 thousand requests, resulting in a $0.05 bill, reaching a total Ad Tracking bill of $0.14._

### Creative Builder Blueprint Management

The Creative Builder Blueprint Management subsection details the costs related to the blueprint management process, the blueprints' storage is charged based on how many blueprints you have and for how long they were stored. There is a free quota of 1000 requests available for the other services in this subsection, after which you will be charged per request.

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption><p>Creative Builder Blueprint Management.</p></figcaption></figure>

_**Example**: As you can observe in the image, except for storage, all other services have a free quota of 1,000 requests. Since none of them have reached the quota, there will be no charges related to them. Regarding storage, it was billed at $0.01 per blueprint per month (720 hours). Nearly 1,300 blueprint-hours were consumed in a month, which is equivalent to keeping 2 blueprints stored for a month, resulting in a $0.02 bill for storage._

### Creative Builder Build Management

This subsection details the costs related to the Builds management process. There is a free quota of 1,000 requests for all listed services, except for storage. After exceeding this quota, you will be charged per request. Storage is charged based on the number of builds you have stored and the duration of storage on the platform. Deleting actions are not charged.

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption><p>Creative Builder Build Management</p></figcaption></figure>

_**Example**: You will notice that in this picture, except for the storage, there were no charges as the listed services had a free quota of 1,000 requests, which was not exceeded. The storage was charged $0.01 per build per month (720 hours). Nearly 5,000 build-hours were consumed, which is equivalent to keeping almost 7 builds stored for a month, resulting in a $0.07 bill._

### Creative Group Management

The Creative Group Management subsection outlines the costs associated with managing creative groups. Deletion actions incur no charges. Each service offers a free quota of 1,000 requests, except for storage. Once the free quota is exceeded, charges apply per request. Storage costs are based on the number of creative groups stored on the platform and the duration of their storage.

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption><p>Creative Group Management</p></figcaption></figure>

_**Example**: In this picture, you will notice that there was a free quota of 1,000 requests for each service, except for storage. Since the quota was not exceeded for these services, there will be no charges. Storage was billed at $0.10 per creative group per month (720 hours). Nearly 60,000 creative group hours were consumed, resulting in an $8.39 bill, which is equivalent to almost 84 creative groups stored for a month (720 hours)._

### Creative Management

This subsection provides details on the costs associated with creative management. Deletion actions are free of charge. Each service, except storage, includes a free quota of 1,000 requests; charges are applied per request beyond this limit. Storage costs are based on the number of creatives and the duration for which they are stored on the platform.

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption><p>Creative Management</p></figcaption></figure>

_**Example**: In the picture, you can observe that there was a free quota of 1,000 requests per service, except for storage. Since none of these services exceeded the quota, there will be no charges. Storage was billed at $0.10 per creative per month (720 hours). With a little more than 74,000 creative-hours consumed, the resulting bill is $10.30, which is equivalent to storing almost 103 creatives for a month (720 hours)._

### Domain Management

This subsection contains billing information related to the domain management process. There is a free quota of 1,000 requests for the listing domains service, after which charges will be applied per request.

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption><p>Domain Management</p></figcaption></figure>

_**Example**: You will notice in the image that the only service used was the domain listing, this service had a free quota of 1000 requests, since the quota was not exceeded, there will be no charges._

### Exchange Review Management

The exchange review management subsection contains billing information related to the exchange review process, including refreshing the exchange review status and sending an ad for exchange review. Each will be charged per request after exceeding the free quota of 1,000 requests per service.

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption><p>Exchange Review Management.</p></figcaption></figure>

_**Example**: In this picture, you will notice that there was a free quota of 1,000 requests for refreshing the exchange review status. After exceeding this quota, the service was billed $0.01 per 1,000 requests. With nearly 15,000 requests made, the resulting bill is $0.15. The other service did not exceed the free quota, so there will be no charges for it._

{% hint style="info" %}
All products generate metrics once you start using them. These metrics are charged and are crucial for understanding your BMS platform usage and performance. The monitoring tab is responsible for these metrics and will display the related bill.\
BMS is focused on transparency and will show you the costs for all features within each product.
{% endhint %}
