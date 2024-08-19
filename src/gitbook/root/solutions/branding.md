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

# Creating a Branding Campaign

Branding campaigns aim to increase the awareness of a given brand and bring the user back to your website. All campaigns have 3 main components: a Target (what is the subset of the population that should see your campaign), a Budget (how much do you want to spend daily on the campaign) and a list of Ads (what the users should see).

To create a branding campaign you must already have your ads set up in our Ad Server. [Check how to do that here.](../product-documentation/ad-server/ads/) With the ads ready, here is an overview:

1. [Create a new campaign](branding.md#creating-a-new-campaign)
2. [Define a daily budget](branding.md#defining-a-budget)
3. [Configure one or more targets](branding.md#configuring-one-or-more-targets)
4. [Choosing which ads to show](branding.md#choosing-which-a-ds-to-show)
5. [Turn on the campaign](branding.md#turn-on-the-campaign)
6. [Watch the impressions and clicks in real-time](branding.md#watch-the-impressions-and-clicks-in-real-time)
7. [Check metrics](branding.md#check-metrics)

### Creating a new campaign

In our Home Page, click on <img src="../.gitbook/assets/image (2) (2).png" alt="Campaigns" data-size="line"> and then <img src="../.gitbook/assets/image (255).png" alt="" data-size="line">, fill in the details paying attention to:

* The domain you choose must be the same domain selected when the ads were created.
* The bid price you choose directly influences the quality of the inventory you will get access to. The more mainstream a website is, the more expensive it becomes. We recommend opting for a variable bid price so that you can get impressions in a wide variety of websites paying the market rate for each. The $0.50 to $1.50 is a good starting point.
* You can schedule your campaign to begin or finish at specific dates, but if you choose to have it starting in the future, you won't see any metrics or real-time data right away. We recommend setting up and testing the campaign first, then scheduling it for a future time.
* You can leave the other fields with their default values. More details on how to optimize and further configure the campaign can be [found here](../product-documentation/demand-side-platform-dsp/).

After saving the campaign, select it on the list to continue its configuration.

### Defining a budget

For your campaign to run, we need to know how much you are willing to spend daily. The system will spread your impressions throughout the entire day. In the Configuration > Budget panel, simply type the amount and save it.

New accounts are limited to spending $30 per day per campaign. If you need more than this later, you can submit a Quota Increase Request and after review your limit will be increased.

### Configuring one or more targets

With a daily budget allocated, we need to know who you want to target. To create the first target, in the Configuration > Targets panel, click on the <img src="../.gitbook/assets/image (5) (2) (1).png" alt="Create Target" data-size="line"> button.

You can specify your target audience by using four main filters:

* Location based: You can choose who to show ads to based on where these users are located by either specifying the country and region or by adding geofences around specific addresses.
* Content based: You can choose what websites to display your ads at based on the content of the website including the language it was written in, the categories that identify what it is about, specific domains, and keywords present in the URL.
* Device based: You can choose what devices to display your ads in based on the device characteristics such as its operating system, browser, and device type among others.
* Inventory based: You can choose what inventory to purchase based on what ad exchange is providing the ad spaces, the position of the ad space on the website, or its past viewability.

Please note that the more filters you apply, the more specific your audience will become. We recommend that you play with these settings until you find the right targeting options that work for your campaign. You can clone existing targets to make it easier to change some aspects and monitor their performances.

### Choosing which ads to show

With targets defined now it is the time to select the ads you want to show to your audience. In the Configuration > Ads panel, click on <img src="../.gitbook/assets/image (5) (2) (1).png" alt="Create Ad" data-size="line">.

You will be presented with a list of all ads that match the campaign's domain. You can refine the search and use the <img src="../.gitbook/assets/image (14) (2).png" alt="Preview" data-size="line"> to preview the ad.

Check all the ads you want to select then click on <img src="../.gitbook/assets/image (13) (2).png" alt="" data-size="line"> to confirm.

You can remove or select more ads at any time.

**Note**: If your ad has been recently created, it might have a <img src="../.gitbook/assets/image (16) (2).png" alt="Issue Sign" data-size="line"> sign, it can be related to not having a rule configured or pending approvals on Ad Exchanges. You can check what is the issue by hovering the cursor over the warning sign.

### Turn on the campaign

It is time to start the campaign! On the main table just switch it on by flipping the Enable toggle <img src="../.gitbook/assets/image (17) (2).png" alt="switch" data-size="line">.

**Note**: You can **enable** or **disable** your campaign at anytime and also make real time changes while having the campaign active. Any changes you make will take up to 15 seconds to take effect.

Please check that the campaign has a green check: <img src="../.gitbook/assets/image (48) (1).png" alt="" data-size="line">. This symbol will change to a <img src="../.gitbook/assets/image (16) (2).png" alt="Issue Sign" data-size="line"> sign if there are any issues that would prevent the campaign from running effectively. By hovering the cursor over the exclamation mark you will be presented with the reason for the warning.

{% hint style="info" %}
_Our bidding works by crossing the information of your configured campaign's settings and bid set, so you will be getting impressions based on your campaign's configuration only._
{% endhint %}

### Watch the impressions and clicks in real-time

When your campaign is active, you can go to the **Real Time** panel and check your campaign events happening in real time:

* Impressions: The bid placed won the auction and your campaign got the right to display the ad to the end user.
* Deliveries: The end user's Browser downloaded your ad from our Ad Server.
* Displays: Your was displayed inside the end user's browser.
* Views: The end user has seen at least 50% of your ad on his screen for 1 second at least.
* Clicks: The end user clicked on your ad.

You can click on the <img src="../.gitbook/assets/image (14) (2).png" alt="Preview" data-size="line"> button to get more details about each event.

You can learn more about real-time events on the [Real Time Tab Documentation page](../product-documentation/demand-side-platform-dsp/real-time-tab.md).

### Check metrics

While real-time events are kept for 15 minutes, you can check the campaign metrics for any time interval. Metrics can take up to 5 minutes to display the most recent data.

In the metrics tab you can explore several metrics, grouping values by specific fields, change visualization between charts and tables, change time range, and download the data to analyze it in your own device.

Most relevant metrics

* Budget Spent - indicates how your budget is being spent over time.
* Impressions and CPM - indicates how many impressions are being made and what is the Cost-per-Mille.
* Viewability - indicates the percentage of impressions that are actually being seen.
* Clicks and CPC - indicates how many clicks are being made and the Cost-Per-Click.

Grouping options

* Campaign: Good to compare the performance of multiple campaigns.
* Ad: Check which Ad is performing better and make adjustments or remove them.
* Target: Be able to see how your targets are performing and which of them can be improved or disabled.
* Exchange: Get to know how the exchange is behaving and which is worth your spending your budget in.

Visualization options

* Metric Cards: This manner is an easier way to view your metrics and compare them with others since they will be showing you a graphic and pointing to each group chosen.
* Data Table: By selecting this visualization method, you can either check on your screen the data requested or download it as .csv and then make your own filters and work with the values shown. To download it simply select the visualization method and then click on <img src="../.gitbook/assets/image (18) (2).png" alt="" data-size="line"> to start downloading your metrics.

You can also check your metrics through the **Overview** page, you can reach it through the Home page or Campaigns page, simply click on <img src="../.gitbook/assets/image (20) (2) (1).png" alt="" data-size="line">, there you can choose a campaign and check its metrics in a broader view.

All metrics have a <img src="../.gitbook/assets/image (19) (2).png" alt="" data-size="line"> to help you identify what that metric is about.

You can learn more about metrics in the [Metrics Tab Documentation page](../product-documentation/demand-side-platform-dsp/metrics.md).
