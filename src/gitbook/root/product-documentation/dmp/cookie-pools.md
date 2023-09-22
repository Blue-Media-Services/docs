---
description: >-
  Find out what a Cookie Pool is, how to create, manage and install it on your
  site.
---

# Cookie Pools

A Cookie Pool is a collection or database of user cookies that is maintained by an organization, typically an advertising or marketing company. Cookies are small pieces of data that are stored in a user's web browser when they visit a website. These cookies can contain information about the user's online behavior, preferences, and interactions with websites and online services.

In the context of digital advertising and marketing, a cookie pool can serve several purposes:

1. **Audience Segmentation:** Advertisers and marketers use cookie pools to segment users into different groups based on their interests, behaviors, demographics, or other criteria. This segmentation allows for more targeted and personalized advertising campaigns.
2. **Retargeting:** Cookie pools are often used for retargeting campaigns. When a user visits a website and leaves without making a purchase, for example, their cookie data can be added to a pool. Later, that user can be shown ads related to the products or services they viewed on other websites as they browse the internet.
3. **Ad Personalization:** Cookie pools help in delivering personalized ads to users. By analyzing the data stored in the cookies, advertisers can determine which ads are most relevant to specific users, increasing the chances of engagement.
4. **Analytics and Measurement:** Advertisers use cookie data to track the performance of their campaigns. They can measure metrics such as click-through rates, conversion rates, and user engagement to assess the effectiveness of their advertising efforts.
5. **Frequency Capping:** Cookie pools also enable advertisers to set frequency caps, which limit how often a particular ad is shown to a user within a certain time frame. This helps prevent users from being bombarded with the same ad repeatedly.

### <mark style="color:blue;">Creating a Cookie Pool</mark>

1. In the Cookie Pool area, click on the **"+ Cookie Pool"** button.
2. Fill the details:
   * Name - how you want to call this cookie pool
   * Tag - for your organization
   * Domain -  the main domain in which you want to collect cookies
   * Exchanges&#x20;
   * TTL - The number of days after which cookies without use are removed from the pool.
   * Max Size - The maximum size that this pool can grow to. Zero if i is unbounded. After a pool is full, no new cookies will be accepted.

### <mark style="color:blue;">Setting up your Cookie Pool</mark>

After creating your Cookie Pool, select to receive the **install instructions**. How you can do this installation:&#x20;

1. Installation in the header of your site&#x20;

Copy the code below and paste it on the pages of your website where you want your users to be added to the pool. Paste the code as high up as possible in the page's `<head>` tag.

2. Tag Manager

* Learn how to install your Cookie Pool using BMS Tag Container
* Learn how to install your Cookie Pool using Google Tag Manager (GTM)

### <mark style="color:blue;">Cookie Pools Metrics</mark>

In the metrics area, you can track the metrics of your cookie pool. The information provided is:

* **Expiration Count -** The number of cookie expirations
* **Max Size -** The maximmum number of cookies allowed inside the pool.
* **Size -** The number of cookies inside the pool.
* **Sync Count -** The number of cookie synchronizations.
* **Time until Expiration -** How long it will take until cookies in the pool expire.

