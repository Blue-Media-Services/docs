# Métricas de DSP

## Campaign Metrics

In the Campaigns section, a metrics tab containing data is available, following our metrics standard, when not selecting any of your campaigns, this tab will show you an account-wide of all your campaigns. Selecting more than one campaign will show a comparison between the selected campaigns, and selecting only one campaign will enable the group by feature with four options:

* **Campaign**: This option will display all the available metrics for the selected campaign.
* **Ad**: This option will display a data comparison between the ads on the selected campaign, allowing you to gather information about your audience. This information can be used to create more engaging ads in the future.
* **Target:** This option will display a data comparison between your campaign's targets, allowing you to gather information about your audience. This information can be used to configure more precise targets in the future.
* **Exchange**: This option will display a data comparison between the ad exchanges used to run your campaign, allowing you to gather data on which ad exchange has been more effective for your campaign.

Additionally, when reviewing metrics, you can always use the <img src="../../.gitbook/assets/image (462).png" alt="" data-size="line"> to access our articles about a specific metric.

{% hint style="info" %}
You can learn more about how metrics are handled by visiting the [Metrics page](../metricas.md).
{% endhint %}

Below you can find all the metrics that our DSP product is responsible for.

### Campaign Active

This metric indicates whether your campaign has been active or not, and when the campaign has been active within the selected time frame.

<figure><img src="../../.gitbook/assets/Campaign Active.png" alt=""><figcaption><p>Campaign Active Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe that the campaign has been active during the period June 16-24. This metric shows results only when a campaign has been active. If there are no results in this metric, it means that the campaign was disabled during that period._

### **Bids and Bid Win %**

This represents the number of bids placed on auction. It does not mean you have won the auction, only that you placed a bid based on your bid pricing. The ratio of successful bids to total bids placed is an important metric, as it will be decisive for knowing when to raise your bid price or change your strategy. This metric will help you understand how many bids you win.

<div><figure><img src="../../.gitbook/assets/Bids and Bid Win.png" alt=""><figcaption><p>Bids Metric</p></figcaption></figure> <figure><img src="../../.gitbook/assets/Bids and Bid Win2.png" alt=""><figcaption><p>Bid Win% Metric</p></figcaption></figure></div>

_**Example:** The graph shows the volume of bids in a campaign over six days (June 10-16). The number of bids varies considerably, with the peak on June 11th (2,000 bids) and the lowest number on June 14th (less than 500 bids). On June 16th, the highest bid and the lowest bid are equal. You can see from these metrics that not all bids were successful<mark style="color:purple;">.</mark> By making strategic changes based on bid pricing and targets, you can reach a higher win rate. It may be that the audience you were targeting is more expensive than the bid set._

### Bid Price Target

This metric shows the bid price configured for your campaign. There are three visualization options: minimum, maximum, and average. The displayed value is for 1,000 bids

<figure><img src="../../.gitbook/assets/Bid Price Target.png" alt=""><figcaption><p>Bid Price Target Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe that the average bid price for this campaign was $50 per bid for the defined time frame (June 17-24). If you set a variable bid price between $0,0001 and $100 you will observe that this metric will show you the bid price targeted, on the maximum visualization you will see the card shows the maximum bid value, on the minimum, it shows the minimum value, and on the average, the average value configured for your campaign._

### **Bid Price Effective**

This metric indicates the prices placed on bids and shows how much you are actually paying on each auction. You can make adjustments to spend less or more budget based on how much you are paying if you are using our variable bid pricing. You can check how our intelligent bidding is affecting your costs.

<figure><img src="../../.gitbook/assets/Bid Price Effective.png" alt=""><figcaption><p>Bid Price Effective Metric</p></figcaption></figure>

_**Example:** You can see on this graph that the average bid price ranged from $0.50 to $1.00. When placing bids on uncontested domains, you are likely to pay an average or even the minimum price for the auction, rather than the maximum. However, in highly contested domains, you may need to increase your bid or pay close to the maximum. This is largely influenced by the current price of the auction. In this metric, we observed that at some points, we encountered domains or target configurations that required higher bid prices, resulting in an increase of nearly $1.00._

### Device Count

This metric shows the number of unique devices from which you have received an impression. Each device is counted only once.

<figure><img src="../../.gitbook/assets/Device Count.png" alt=""><figcaption><p>Device Count Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe that the ad was delivered to 4 different devices on June 17th, to 3 devices on June 18th-19th, and 1 device per day until the end of the defined time frame ( June 17-24). If a user inside the parameters of your target receives your ads on his PC, this will count as a unique device, if the same user receives your ads on his smartphone it will count as another device._

### Device Frequency

This metric displays how many impressions your ads receive from the same device.

<figure><img src="../../.gitbook/assets/Device Frequency.png" alt=""><figcaption></figcaption></figure>

_**Example:** A user within your target parameters can be impacted multiple times by the same ad on the same device. This metric counts how many times the ad was displayed on the same device. In this graph, you can observe that on June 17th, your ad was delivered to the same device just over 10 times, while on June 18th, this number increased to about 15 times per device._

### **Impression**s

After winning a bid, you earn the right to publish the ad on the domain where you placed the bid. An impression is based on a user having your ad downloaded on the domain's page.

<figure><img src="../../.gitbook/assets/Impressions.png" alt=""><figcaption><p>Impressions Metric</p></figcaption></figure>

_**Example:** The graph shows the volume of impressions during a period of six days (June 10-16). There was a peak of nearly 700 impressions on June 11th. Once you start your campaign, if your bids are successful, you will begin to receive impressions based on winning bids. A campaign focused on branding aims to get as many impressions as possible, since your goal is to reach a larger public._

### **Impression Price**

The prices paid on successful bids. Know exactly how much you are paying for a successful bid.

<figure><img src="../../.gitbook/assets/Impression Price.png" alt=""><figcaption><p>Impression Price Metric</p></figcaption></figure>

_**Example:** It is useful to know when the impression is getting expensive. In this metric, you can see that the impression price has met $2.00. This can happen when the targets are not broad enough, causing you to spend more budget to get 1000 impressions. Make adjustments based on your campaign's objective. If you are targeting a more specific audience, your impression price might be a bit high._

### **CPM**

This is the cost per every 1000 impressions. It can serve as a baseline to know whether your campaign is reaching the targeted CPM. Based on your CPM strategy, note that the CPM is not the total cost of your campaign. For that, you will have to check your Budget Spent Metric.

<figure><img src="../../.gitbook/assets/CPM.png" alt=""><figcaption><p>CPM Metric</p></figcaption></figure>

_**Example:** In this graph, you can see that the CPM has reached over $3.50 due to a change of targets. If there is a very specific audience targeted, you may need to spend a bit more to win bids on disputed domains. If you start a branding campaign focused on reaching a maximum of $4.00 per 1000 impressions, you will need to check if your campaign is getting enough bid wins to generate impressions. Make the necessary changes, such as slightly adjusting your targets or increasing your bidding price._

### **CPC**

This metric represents the budget spent for each click. Many campaigns prioritize clicks, and CPC indicates the cost per click. If your campaign emphasizes clicks, it's essential to monitor both the CPC and the Budget Spent metric to determine the overall effectiveness and cost efficiency of your campaign.

<figure><img src="../../.gitbook/assets/CPC.png" alt=""><figcaption><p>CPC Metric</p></figcaption></figure>

_**Example:** In this metric, you can observe that the cost per click varies for each ad, reaching a maximum of nearly $1.30. This fluctuation may be influenced by factors such as when the ad is displayed, the time window you are targeting, and whether the creative is compelling to your intended audience._

### Cost Per Page Load

This metric shows a median of how much of your budget has been spent for each page loaded.

<figure><img src="../../.gitbook/assets/Cost Per Page Load.png" alt=""><figcaption><p>Cost Per Page Load</p></figcaption></figure>

_**Example**: After installing the page loading tracking tag, this metric will show you a median of how much each page load has cost you in the defined time frame. In this picture, the defined time frame was 3 days, divided into 6-hour periods, you will notice that on Aug 21, at 12:00 PM the average cost per page load was nearly $1.60, this was the maximum cost on the period, after that there is an oscillation that stays between $0.50 and $1.50._

### Budget Available

This metric shows how much of your budget is still available for a campaign, it will show new values as the budget is being spent.

<figure><img src="../../.gitbook/assets/Budget Available.png" alt=""><figcaption><p>Budget Available Metric</p></figcaption></figure>

_**Example:** In this graph, you can see that there was a daily budget of $30, which was completely spent each day from June 21st until June 24th. By following this metric, you will be able to observe how much of your budget remains available for your campaign._

### Budget Daily Limit

This metric displays the value defined as the daily budget within the specified time frame.

<figure><img src="../../.gitbook/assets/Budget Daily Limit.png" alt=""><figcaption><p>Budget Daily Limit</p></figcaption></figure>

_**Example:**_ Use the data provided in this metric to understand the daily budget limit configured at the time. In this picture, the defined time frame was 3 days, divided into 6h periods. You will notice that the configured daily budget limit was $10.00, and this setting has remained unchanged.

### **Budget Spent**

Represents the total budget spent, including media purchases, ad delivery, and bidding activities. This is the overall cost of running your campaign. The campaign is not just based on its bid price, which was established when the campaign was created.

<figure><img src="../../.gitbook/assets/Budget Spent.png" alt=""><figcaption><p>Budget Spent Metric</p></figcaption></figure>

_**Example:** In this metric, you can see that the budget spent per ad has not reached $1.00 since you established our bid pricing below $1.00. If you make any changes during the campaign, the metric will reflect those changes._

### Budget Pace Target

This metric shows the defined budget pace target. It helps you plan the rate at which your budget will be consumed.

<figure><img src="../../.gitbook/assets/Budget Pace Target.png" alt=""><figcaption><p>Budget Pace Target Metric</p></figcaption></figure>

_**Example:** If you have a daily budget of $10, this metric will show the pace at which this budget should be spent over the course of your campaign. In this graph, you can observe that the daily budget was under $5 from June 16th to June 23rd, then on June 24th, the daily budget increased to $15._

### Budget Pace Effective

This metric shows you the actual race at which your budget is being consumed. It allows you to gather information on which hours of the day or days of the week, your ads spent your budget.

<figure><img src="../../.gitbook/assets/Budget Pace effective.png" alt=""><figcaption><p>Budget Pace Effective Metric</p></figcaption></figure>

_**Example:** In this graph, you can observe the budget pace adjusted to spend all the budget defined for that period (June 21-24). The budget pace effective metric will show you how this budget is being spent effectively and during which hours or days it has been spent._

### **Budget Spent on Impressions**

This metric represents the total budget spent on media purchases and reflects the expenses incurred for acquiring ad spaces.

<figure><img src="../../.gitbook/assets/Budget Spent on Impressions.png" alt=""><figcaption><p>Budget Spent on Impressions Metric</p></figcaption></figure>

_**Example:** In this graph, you can see that the budget spent was a little high. However, after making adjustments on the targets, you reached a better average of over $0.75. It is important to know exactly how much you are spending on impressions, to optimize your budget effectively. Impressions are crucial for branding campaigns, as they help reach a wider audience or convey important messages._

### **Budget Spent on Deliveries**

This metric indicates the total budget spent on the ad delivery process, including the costs associated with distributing ads to the target audience.

<figure><img src="../../.gitbook/assets/Budget Spent on Deliveries.png" alt=""><figcaption><p>Budget Spent on Deliveries Metric</p></figcaption></figure>

_**Example:** In this graph, you can see that the average reached was between $0.15 to $0.35. It is important to understand the amount you are spending on deliveries, which is measured by the sum of impressions, deliveries, displays, and views. This will assist you in determining whether the deliveries are meeting your campaign's objectives and enable you to make necessary adjustments._

### Budget Spent Placing Bids

This metric shows how much of your budget the bidding engine has consumed when placing bids for ad spaces.

<figure><img src="../../.gitbook/assets/Budget Spent Placing Bids.png" alt=""><figcaption><p>Budget Spend Placing Bids</p></figcaption></figure>

_**Example:** When you start running a campaign on our platform, the system will start placing bids according to your campaign settings. This metric shows you a sum of how much of your budget has been consumed placing bids. In this picture, you will notice that the defined time frame was 1 week divided into daily periods, from Oct 16 until Oct 18, the consumption related to placing bids was nearly $0.50 per day, after that, you will observe an increase of this value until almost $2.00 on Oct 21, and then it decreases again._

### Budget Spent with Recommendations

This metric shows how much of your budget was spent based on recommendations. It will only appear if you are using a recommendation model for this campaign.

<figure><img src="../../.gitbook/assets/Budget Spent with Recommendations.png" alt=""><figcaption><p>Budget Spent with Recommendations Metric</p></figcaption></figure>

_**Example**: In a context where you have a retargeting campaign designed to engage users on your website, the budget allocated to recommending products from your catalog to these users is shown in the "Budget spent on recommendations" metric. The graph displays a one-week time period, with each point corresponding to a day and the budget spent on recommendations. You can see that on June 24th, the budget spent on recommendations was almost $0.07, with a considerable drop on June 28th._

### Rejected Bids

Bids can be rejected for many reasons, such as the ad not being in compliance with the publisher's ad rules. You can use the real-time tab or our event pipes to obtain more details about the reason your bids are being rejected. This metric shows the number of bids that were rejected within the defined time frame.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption><p>Rejected Bids</p></figcaption></figure>

_**Example**: In this graph, you can see a count of the rejected bids within a defined time frame, which here was 1 day, divided into 6-hour periods. At 6 AM, a little more than 5,000 bids were rejected; and then it remains stable between 12 PM and 12 AM, with nearly 2,500 bids rejected per period; and then it goes to nearly 5,000 rejected bids in the next period._

### Losing Bids

Bids are only lost when they are outbid, meaning that someone has made a higher bid for the same opportunity and won the auction. This metric shows the number of bids that were lost.

<figure><img src="../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>Losing Bids</p></figcaption></figure>

_**Example**: In this graph, the defined time frame was 1 day, divided into 6-hour periods. It is possible to notice that at 6 AM, nearly 800 bids were lost, and that in the next periods, this number decreases until nearly 100 lost bids at 12 AM; and then, this number increases to almost 500 lost bids in the next period._

### Losing Bid Prices

This metric represents the value of the bids that were lost. Combined with the Minimum Price to Win metric, it provides valuable data about your ideal bid price.

<figure><img src="../../.gitbook/assets/image (4) (4).png" alt=""><figcaption><p>Losing Bid Prices</p></figcaption></figure>

_**Example**: In this graph, the defined time frame was 1 day divided into 6-hour periods. In the first 3 periods, you will notice that the bid price of the bids we lost was nearly $0.40 per mille, and at midnight, this value increases to almost $1.40 per mille, meaning that even higher bids were losing auctions._

### Minimum Price to Win

This metric represents the minimum value that would be required to win bids that were lost. Combined with the Losing Bid Prices metric, it provides valuable data about your ideal bid price.

<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption><p>Minimum Price to Win</p></figcaption></figure>

_**Example**: This graph has a defined time frame of 1 day, divided into 6-hour periods. It is possible to notice that in the first period, at 6 AM, the minimum bid price to win was nearly $1.2 per mille. Taking into consideration the previous graph, you will learn that our losing bids at the same period were of nearly $0.40 per mille, meaning a cost difference of $0.80 per mille, which explains why we had so many losses at this period._
