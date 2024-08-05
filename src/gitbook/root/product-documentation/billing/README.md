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

# Billing

As BMS is a self-service platform, our billing works differently, offering more transparency in how your bills are presented. Most platforms do not provide detailed information about each service used, which can give the impression that some services are not being charged. However, it is important to understand that every access, API call, and file stored on a platform incurs a cost.

BMS believes that showing users the exact amount they are paying for each service is essential for transparency. By doing this, users can identify where most of their money is being spent and make strategic decisions based on that information.

_**Example:** when checking the menu in a restaurant, the restaurant typically does not provide the cost of each individual ingredient in a dish; it only displays the full price. However, in BMS, each ingredient, the amount requested, and the cost for each are all transparently displayed, allowing you to decide which ingredients you will consume._

All our products will include detailed information on the cost of each service used. BMS will not charge for features or products you are not using.

To access your bills, click on the dropdown menu on your account, and then click on <img src="../../.gitbook/assets/image (3).png" alt="Billing" data-size="line">.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Accessing Billing</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption><p>Bills</p></figcaption></figure>

Once you access the bills page, you will be presented with the bills for the current month.

## Summary

* Account ID - Current Account ID's Bills
* Period - The period in which the current bills are being selected
* Last Update - Shows when the charges per service were last updated.
* Status - The current status of your selected bill. Once the bill for the selected month is closed, it will present the current status.

## Estimated Total

* Total before taxes and discounts - Total cost before including taxes and discounts for the services.
* Discounts - If BMS provides any discount, it will be shown.
* Tax - Should any tax be included in your payment.
* Grand Total - If any discount or tax is included, the grand total will present the sum of all values.

## Charges per Service

In this section, all our products will be listed. After clicking on <img src="../../.gitbook/assets/image (4).png" alt="Dropdown menu" data-size="line"> , the list will expand to display all charges related to that product. You can check each product separately or click on <img src="../../.gitbook/assets/image (5).png" alt="Expand All" data-size="line"> to view all products at once.

By expanding a product, you will see a detailed view of each service used within that product. This option provided by BMS allows users to control their expenses and identify areas to avoid unnecessary use. Through BMS's transparency, users can check all services used, the total price, and the amount of usage processed.

## Billing Models

The BMS has two types of charging: **Discreet Billing** and **Continuous Billing**.

### Discreet Billing

Discreet billing refers to a billing model where charges are applied for specific actions or events as they occur, rather than on a recurring or flat-rate basis. This model focuses on transparency and precision in billing, ensuring that users pay exactly for the resources and services they consume. For instance, when accessing a product and performing actions such as creating, viewing, or requesting reports, each action will be counted as an API call or request. Since BMS is a transparent platform, all requests will be shown on the bill for the corresponding product.

BMS's platform consists of multiple APIs. Each time you access a product and perform any action, it counts as one API call, indicating that the API has been used. BMS refers to an API call as a request, and it will be reflected in your billing under the corresponding product you accessed and interacted with.

_**Example:** If you access the media library and upload media, it will count as one request. Similarly, downloading that media will also count as one request. After uploading an image, if you send the image link to someone else and they access the image, you will also be charged because the image is hosted on BMS's servers and linked to your account._

Below you can find some requests that fit our discreet billing model.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Requests Example</p></figcaption></figure>

_**Example:** The lines "Get Ad - First 1000 - free" and "Get Ad - After 1000 - $0.01 per 1000" refer to the same service, meaning that you will have 1000 requests for free and, after that, you will be billed on USD 0.01 per 1000 requests._

### Continuous Billing

As part of discreet billing, when you access, create, and manage features on BMS, any uploaded media, created campaigns, ads, and creatives stored on BMS will consume space on BMS's servers. BMS incurs costs for the usage of this space, and even though all data is stored in the cloud, there is a cost associated with it that the user must pay.

While all platforms charge for the space used, BMS stands out by transparently showing exactly where the user is consuming space. This transparency enables users to make informed decisions about using less of a product or opting to store media on their own servers to avoid those charges.

This billing model is based on the real-time usage of BMS, accounting for the time a feature is actively used. For instance, a campaign active for an entire month will be charged for 720 hours of usage. If you run two campaigns for half a month and then deactivate them, you will also be charged for 720 hours since the combined usage of both campaigns will total 720 hours. BMS measures the usage time in seconds, but for billing purposes, it is converted to hours. Therefore, you will only be charged for the actual time a feature is in use.

The creations consume space because they are stored on the BMS server. Therefore, the charge will be based on the amount of space used.

_**Example:** Once you upload a media file of 1MB, BMS will start tracking how long the media is stored and will charge for this media as long as it stays on BMS's server. If you keep 1MB of media for a month, the bill will be based on the entire period in seconds and the amount of data stored in total. If you delete the media, BMS will stop charging for it, as it is no longer consuming space._

## Metrics

All metrics in our products are tracked and charged under the Monitoring tab. As soon as any metric starts receiving and storing information, it will be recorded in the Monitoring tab. This is because the monitoring product is responsible for capturing and managing all events from the platform.

Metrics are a valuable feature that incurs charges based on usage. While every platform has its own way of charging for this feature, BMS ensures transparency by displaying which metrics are being used and how much data is being collected for each product. This allows you to optimize usage and minimize costs.
