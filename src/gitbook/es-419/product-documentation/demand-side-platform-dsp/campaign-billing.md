# Facturación de Campañas

The Campaigns billing section will contain all billed items related to campaigns, it is divided into 2 sub-sections.

<figure><img src="../../.gitbook/assets/image (566).png" alt=""><figcaption><p>Campaigns Billing Section</p></figcaption></figure>

{% hint style="info" %}
At BMS, it prioritizes transparency by displaying every detail of your bill. Visit our [Billing Home](../billing.md) to understand how the bills are structured.
{% endhint %}

## How is your billing composed?

When creating and starting a campaign, it is necessary to use multiple products and features from our platform in order to have everything set to start the campaign, note that the campaign's billing is not only based on the daily budget set.

### Billing X Budget

Our Billing works based on the usage of each product, it is the effective cost for each product based on the usage, metered by each request sent to an **API**, **storage**, and **media**.

### Storage

When running a campaign, multiple products are used to build its components. As a result, the storage for each creative, creative group, ad, and media item will incur charges. In cases where the account accumulates too many of these items, there could be a significant impact on the monthly billing. Therefore, performing regular clean-ups of unused items is a good practice to maintain a manageable billing balance.

**Example:** Even when a campaign is inactive, charges may still apply because the creatives and ads created for that campaign continue to incur storage costs.

### Media

All media uploaded to the library incur storage and download request costs. Each time an end-user views your media in a campaign, a cost is generated for both storage and download. These costs vary based on the size of each media file, as they consume storage space on BMS servers. To help manage these expenses, consider using media hosted on your own servers.

**Example:** A media that has a 3mb size will have a different cost from a 5mb media size, by hosting that media on your own server, BMS will not charge for that media.

### Daily Budget

The daily budget set for a campaign functions like a gas pedal, helping you control how much you intend to spend. The actual amount spent by the end of the day may vary based on target configurations, bidding settings, and the media used in the campaign.

Upon setting your daily budget, it is used on four different types in order to fully delivery a campaign: **Impressions**, **Deliveries**, **Placing Bids**, and **Recommendations**.

#### Budget Spent on Impressions

This budget is spent based on the bids won, with the amount paid to the publisher for the right to display ads on their website. On the billing side, this is represented as the media cost (the sum of all winning bids) plus a 20% platform fee.

<figure><img src="../../.gitbook/assets/image (920).png" alt=""><figcaption><p>Budget Spent on Impressions Metric</p></figcaption></figure>

**Example:** In this case, the budget spent on impressions were over $0.50 to a maximum of $0.75, this metric will be shown at the Budget Management and Media as the Media Cost, upon removing the 20% platform fee, it is possible to match the values.

<figure><img src="../../.gitbook/assets/image (835).png" alt=""><figcaption><p>Budget Spent on Impressions Billing</p></figcaption></figure>

#### Budget Spent on Deliveries

This budget pertains to the total delivery cost of an ad, which includes the combined expenses of Ad Server, Monitoring, and Media. The Ad Server cost covers the API requests needed to deliver the ad, Monitoring costs capture metrics and display them on the dashboard, and Media costs cover the downloading of associated media. On the billing side, these costs appear under **Ad Server**, **Media**, and **Monitoring**. This cost may vary based on the size of the media; larger media files will result in higher expenses.

<figure><img src="../../.gitbook/assets/image (836).png" alt=""><figcaption><p>Budget Spent on Deliveries Metric</p></figcaption></figure>

**Example:** On this metric you can see that hourly it is being spent over $0,01 up to $0,025 on deliveries only, this value will be deducted from the daily budget, even though it is not related to the bidding itself.

#### Budget Spent Placing Bids

This cost is associated with the operational expense of placing bids. Each time a bid is made, it aligns with the campaign’s targets, requiring the system to filter the entire available inventory based on the campaign's preferences to ensure accurate bidding. This process incurs charges, though they represent a small percentage of the total daily budget. On your billing statement, the Real-Time Bidding section will include a "Bids Placed" line item, which corresponds to your campaign's bid placement metrics.

<figure><img src="../../.gitbook/assets/image (919).png" alt=""><figcaption><p>Budget Spent Placing Bids Metric</p></figcaption></figure>

**Example:** On this metric, it is noticed that the budget spent for operational costs has been over $0.05 to a maximum of $0.13, this cost will be listed on your billing as the Real Time Bidding, it will match the operational costs of your campaign.

<figure><img src="../../.gitbook/assets/image (918).png" alt=""><figcaption><p>Placing Bids Billing</p></figcaption></figure>

#### Budget Spent on Recommendations

When using Dynamic Banners, you will be charged for using the API call for a recommendation, due to having an operation cost of linking your targets to a recommendation, if a campaign is not using Dynamic Banners, there will be no costs.

<figure><img src="../../.gitbook/assets/image (794).png" alt=""><figcaption><p>Budget Spent with Recommendations Metric</p></figcaption></figure>

**Example:** On this metric, it is noticed that the budget spent was over $0.05 up to $0.08 every 12 hours, which value is deducted from the campaign's daily budget.

## Budget Management and Media

In budget management and media, the bills related to BMS display the current budget availability, the requests generated when you change or set a budget for a campaign, and the media cost plus a 20% BMS tax. The media cost is based on the amount paid to a publisher to display your ad.

<figure><img src="../../.gitbook/assets/image (567).png" alt=""><figcaption><p>Budget Management and Media Items</p></figcaption></figure>

_**Example:** On this bill, a media cost of $4,014.89 plus CPM is noted. This cost is based on $3,345.74, which will be passed on to the publishers who displayed your ad, and an additional $669.15 from the 20% tax for using BMS's bidder. The campaign budget availability was also charged due to exceeding 1,000,000 requests. At a cost of $0.10 per 1,000,000 requests, this totaled $0.72. After adding up all bills, the total cost reached $4,015.61._

## Campaign Management

On the campaign management bill, the costs for any action on the campaign page and for campaign storage will be displayed. Each time you create, enable or disable campaigns, it counts as one request. If the number of requests exceeds 1,000 during a month, there will be a cost. Campaigns are charged even if they are inactive. BMS counts each second a campaign is listed, whether active or not, and converts seconds into hours, charging $0.75 per campaign per month, based on a 720-hour month.

<figure><img src="../../.gitbook/assets/image (568).png" alt=""><figcaption><p>Campaign Management Items</p></figcaption></figure>

_**Example:** In this case, since no requests have reached the first 1,000 mark, there will be no charges for actions performed on the campaigns page. However, since there were campaigns running or listed, a total of 2,201.09 campaign hours were charged, equivalent to about 3 campaigns running for an entire month. This resulted in a total cost of $2.29. Note that campaigns are charged for being listed, whether active or not, so deleting a campaign will stop further charges._

{% hint style="info" %}
All products generate metrics once you start using them. These metrics are charged and are crucial for understanding your BMS platform usage and performance. The [Monitoring Tab](../monitoring/monitoring-billing.md#metric-monitoring) is responsible for these metrics and will display the related bill.\
BMS is focused on transparency and will show you the costs for all features within each product.
{% endhint %}
