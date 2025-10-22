# Account Billing

The account billing section will contain the cost details related to the accounts service, it has only one subsection: organization.

<figure><img src="../../.gitbook/assets/image (324) (1).png" alt=""><figcaption><p>Account Billing</p></figcaption></figure>

{% hint style="info" %}
At BMS, it prioritizes transparency by displaying every detail of your bill. Visit our [Billing Home](../billing.md) to understand how the bills are structured.
{% endhint %}

### Organization

This subsection details the costs related to managing your organization. Deletions are not charged, there is a free quota of 1,000 requests for each service in the subsection, after which a charge per request will apply. Additionally, requests made to the 'get organization' service are counted each time you need information related to your organization, such as when loading the organization page or opening the menu where your organization's name appears.

<figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption><p>Organization</p></figcaption></figure>

_**Example**: In this picture, you will notice that the requests for listing member accounts, which are counted whenever you load your member accounts list on the organization page, did not exceed the free quota, so no charges were applied. However, after exceeding the quota for the 'get organization' service, a charge per request was applied, resulting in a $0.01 bill._

{% hint style="info" %}
All products generate metrics once you start using them. These metrics are charged and are crucial for understanding your BMS platform usage and performance. The [Monitoring Tab](../monitoring/monitoring-billing.md#metric-monitoring) is responsible for these metrics and will display the related bill.\
BMS is focused on transparency and will show you the costs for all features within each product.
{% endhint %}
