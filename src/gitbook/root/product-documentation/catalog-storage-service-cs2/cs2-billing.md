# CS2 Billing

The catalog storage service billing section is available on the billing page. It contains information about every billed item related to CS2 and is divided into 6 sub-sections.

<figure><img src="../../.gitbook/assets/image (314).png" alt=""><figcaption><p>CS2 Billing Section</p></figcaption></figure>

{% hint style="info" %}
At BMS, it prioritizes transparency by displaying every detail of your bill. Visit our [Billing Home](../billing.md) to understand how the bills are structured.
{% endhint %}

Below is an explanation of each of these sections with their respective details.

### Catalog Management

This subsection outlines the costs associated with catalog management. Deletions are free of charge, and each service in this section includes a free quota of 1,000 requests, except for the storage, which is billed based on the number of catalogs stored and the duration of their storage.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 134927.png" alt=""><figcaption><p>Catalog Management</p></figcaption></figure>

_**Example**: In this picture, there were consumed nearly 1,039 catalog-hours, which is equivalent to 1 catalog stored for a month with another catalog stored for a few days, resulting in a $1.08 charge. You can also observe that no charges were applied for the other services consumed since the free quota was not exceeded._

### Import Channel Management

This subsection outlines the costs associated with import channel management. Import channels configured are billed based on the number of import channels configured and the duration of their availability on the platform, import jobs are billed according to how much data they have transferred, there is a free quota of 100 requests for the start import job service, after which charges will incur per request, for the other services on the section there is a free quota of 1,000 requests, after which the services will be billed per request.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 135947.png" alt=""><figcaption><p>Import Channel Management</p></figcaption></figure>

_**Example**: In this picture you will notice that for most services the free quota was not exceeded and therefore no charges were applied to these services, it is also possible to observe that nearly 325 channel-hours were consumed, which is equivalent to having 1 import channel configured for almost two weeks, resulting on a $0.34 charge, you can see that nearly 5 GB were transferred on this period, resulting on a $0.42 bill, after reaching the quota, the listing import jobs service was charged per request, resulting on a $0.28 charge, therefore this customer will be charged on $1.03 for the services on this subsection._

### Recommendation Model

In this subsection, you will find the cost details for the recommendation models. Deletion actions are free of charge, there is a free quota of 1,000 requests for every service on this section, except for the Models Configured, which is billed based on the number of recommendation models you have configured and the duration of their availability and use.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 140608.png" alt=""><figcaption><p>Recommendation Model</p></figcaption></figure>

_**Example**: You will notice that, in this picture, most of the services consumed did not exceed the free quota, and therefore no charges were applied, it is possible to observe that nearly 835 model-hours were consumed, which is equivalent to 1 model configured for almost a whole month, resulting on a $0.87 bill._

### Recommendation Engine

This subsection details the costs related to the use of the recommendation engine, there is a free quota of 1,000 requests, after exceeding this quota, the charge is applied per product recommendation request.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 140715 (1).png" alt=""><figcaption><p>Recommendation Engine</p></figcaption></figure>

_**Example**: In this picture, the free quota was not exceeded, and therefore no charges will incur for the services._

### Product Management

This subsection contains the cost details related to product management. Deletions are free of charge,    except for the storage, every service on this section has a free quota of 1,000 requests, after which you will be charged per request, the storage is billed based on the number of products you have stored and the duration of their storage.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 140958.png" alt=""><figcaption><p>Product Management</p></figcaption></figure>

_**Example**: You will observe, in this picture, there were no charges for the services that did not exceed the free quota, after exceeding the quota the creating products and the patching products services were billed per request, there were nearly 35 thousand creating products requests, resulting in a $0.52 bill, and nearly 35 million patching products requests, resulting in a $ 513.17 bill, you can also notice that almost 208 million product-hours were consumed, resulting in a $28,85 bill, totalizing a $542.55 bill for the services in the section._

### Catalog Tracking

This subsection contains the cost details related to the catalog tracking, every service in this section has a free quota of 1,000 requests, after which you will be charged per request.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 142247.png" alt=""><figcaption><p>Catalog Tracking</p></figcaption></figure>

_**Example**: In this picture, you will notice that a free quota of 1,000 requests was given to each service, after exceeding this quota, the charges were applied based on the number of requests used, there were nearly 151 thousand requests for tracking product events, resulting in a $1.51 bill, and nearly 31 thousand tracking recommendation event requests, resulting in a $0.31 bill, totalizing $1.82 for the services on the section._

{% hint style="info" %}
All products generate metrics once you start using them. These metrics are charged and are crucial for understanding your BMS platform usage and performance. The [Monitoring Tab](../monitoring/monitoring-billing.md#metric-monitoring) is responsible for these metrics and will display the related bill.\
BMS is focused on transparency and will show you the costs for all features within each product.
{% endhint %}
