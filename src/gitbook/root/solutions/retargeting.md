# Creating a Retargeting Campaign

Retargeting is an ad technique that shows ads based on your product catalog to users who previously interacted with your website or app intending to increase conversions.

To help you create a retargeting campaign from the beginning until it's running we've developed this article, here is what we're going to approach for this purpose:

* [Creating and Installing a Cookie Pool](retargeting.md#creating-a-cookie-pool)
* [Creating a Catalog and Import Channels](retargeting.md#creating-a-catalog)
* [Creating, Setting up, and Installing a Tracker](retargeting.md#creating-trackers)
* [Creating Recommendation Models](retargeting.md#creating-a-recommendation-model)
* [Using the Creative Builder to Create Builds and Blueprints](retargeting.md#creative-builder)
* [Creating Creative Groups](retargeting.md#creating-a-creative-group)
* [Creating Ads and Bulk Ads](retargeting.md#creating-an-a-d)
* [Setting Up Rules for Ads](retargeting.md#creating-a-rule)
* [Creating a Retargeting Campaign](retargeting.md#creating-a-campaign)

## Cookie Pool

We start creating and installing a cookie pool on your website, a cookie pool is a database built upon the user's stored cookies. Cookies are small files stored on the user's web browser that contain data about the user's behavior on the internet.

Use the cookie pool feature to gather more data about audience segmentation and enhance campaign performance. Not using it limits data gathering and recommendation models.

### Creating a Cookie Pool

1. On the [BMS homepage](https://console.bluems.com/), in the DMP section, click on Cookie Pools.
2. Click on <img src="../.gitbook/assets/image (36) (1) (1).png" alt="+ cookie pool button" data-size="line"> to create a Cookie Pool.
3. Now you can set a Name and Tags for it.
4. Insert your domain and select the exchanges you desire.
5. Set the period and the size of the cookie pool.
6. Click on <img src="../.gitbook/assets/image (32) (1) (1).png" alt="Save Button" data-size="line"> to save your cookie pool.

### Installing a Cookie Pool

1. On the [Cookie Pools page](https://console.bluems.com/dmp/cookie-pools), select the tab install instructions.
2. Click on <img src="../.gitbook/assets/image (37) (1) (1).png" alt="Copy button" data-size="line"> to copy the cookie pool tag.
3. Add this code to the \<head> tag of the pages where you want your users to be added to the pool.
   * We recommend you ask your website's developer to perform this action.
   * Alternatively, you can install this tag on your website using Google Tag Manager (GTM).

## Catalog Storage Service (CS2)

Once you have created a cookie pool, it's time to build your product catalog. This will enable you to use recommendation models that increase ad conversions by showcasing your products on dynamic banners.

### Creating a Catalog

1. On the [BMS homepage](https://console.bluems.com/), click on Catalogs, in the CS2 section.
2. Click on <img src="../.gitbook/assets/image (38) (1) (1).png" alt="Create Catalog Button" data-size="line"> to create a new catalog.
3. Set a Name and Tags for it.
4. Click on <img src="../.gitbook/assets/image (34) (1) (1).png" alt="Save Button" data-size="line"> to save your changes.

### Creating an Import Channel

1. At the menu on the Right, click on Import Channels.
2. Click on <img src="../.gitbook/assets/image (39) (1) (1).png" alt="+ import channel button" data-size="line"> to start.
3. Here we need to configure the three tabs available for it to be working properly.
   * General Tab
     1. Set a name and tags for your Import Channel.
     2. Select the catalog from where you will import your product data.
     3. Select how often your catalog should be updated to add or edit your products.
     4. Select how often your products must be removed from your catalog.
   * Source Tab
     1. Select the protocol used on the URL from which the products will be imported.
     2. Inform the URL from which the products will be imported.
     3. Select your catalog format between the available options.
   * Mapping Tab
     1. Inform the template model of your catalog, this step may require the help of our technical team.
     2. Click on <img src="../.gitbook/assets/image (35) (1) (1).png" alt="Save Button" data-size="line"> to save your changes.

After completing the steps above, enable the import channel to start working with it, you can also perform a test to confirm that it's working properly, to perform this test, follow the steps below:

1. Select the import channel that you need to run a test for it.
2. Click on <img src="../.gitbook/assets/image (40) (1) (1).png" alt=" Start Button" data-size="line"> to start a manual import.
3. Flag the 'Testing Mode'.
4. Select how many products that should be tested.
5. Set if you want to use the channel's settings for deleting products or if you want to remove them before the test begins.
6. Click on <img src="../.gitbook/assets/image (41) (1) (1).png" alt="Start Button" data-size="line"> to start.
7. Select the import channel you've run the test, and at the jobs tab you can confirm if the channel is working properly or not, in case of any issues with it, they will be displayed in the column "Issues".

### Products

In this section, you will be able to view all your products. Flag the checkbox of the products and go to the details tab to see more detailed information about it, like the offer ID, for example.

## Trackers

Track your audience's website activities using trackers, and utilize the data to create a product recommendation model based on your catalog.

### Creating Trackers

1. On the [BMS homepage](https://console.bluems.com/), click on Trackers.
2. Click on <img src="../.gitbook/assets/image (42) (1) (1).png" alt="+ tracker button" data-size="line"> to add a new tracker.
3. Set the name for your tracker.
4. Setting tags will help you find this tracker more easily.
5. Set the maximum number of users. New users cannot be added once the limit is reached, but existing user's actions will still be tracked.
6. Set the maximum amount of events tracked per user, once the limit is reached, the system will automatically delete the oldest events to make room for new ones.
7. Set how long you want to use these trackers, after this period your tracker activities will be deleted.

### Configuring Trackers

Set events for tracking specific actions of your audience.

1. On the [Trackers page](https://console.bluems.com/dmp/trackers), select a tracker.
2. On the configuration tab, click on <img src="../.gitbook/assets/image (43) (1) (1).png" alt="Add button" data-size="line">, to create an event.
3. Setting a name for your event will automatically set an ID for it.
4. Set the custom data field with the information you want to track, for example: "offerid".
5. Click on <img src="../.gitbook/assets/image (44) (1).png" alt="Add button" data-size="line"> to create an action to be executed after the event has been tracked.
6. Set a name for the action.
7. Choose between a 'Call a Webhook' or 'Track in Catalog' action:
   * For a 'Call a Webhook' action, inform the URL to where the data should be sent. Here you can also choose default and customized activities to be tracked.
   * For a 'Track In Catalog' action, choose the desired catalog, then the activity you want to track, it's also possible to track a customized activity.
8. Click on <img src="../.gitbook/assets/image (45) (1).png" alt="Save button" data-size="line"> to save the action you created.
9. Feel free to add more actions to this event, then click on <img src="../.gitbook/assets/image (46) (1).png" alt="Save button" data-size="line"> again, to save your event.

### Installing a Tracker on Your Website

After creating your trackers, events, and actions, you must install them on your website to start using them. There are 3 install methods available: Script, Pixel, and Redirect.

* Script
  1. On the [Trackers page](https://console.bluems.com/dmp/trackers), select the desired tracker.
  2. Click on the 'Install Instructions' tab, and choose the event you want to track.
  3. Select the Script option.
  4. If you have configured custom data fields, please use the indicated placeholders to inform the values.\
     Here's an example of how the indicated placeholder for your custom data fields might look to you: <img src="../.gitbook/assets/image (48) (1) (1).png" alt=" Custom data field example" data-size="original">.
  5. Click on <img src="../.gitbook/assets/image (49) (1).png" alt="copy button" data-size="line"> to copy the script.
  6. Add this script to your website's code, on the page where the event will be tracked.
  7. You can also use a tag manager, like Google Tag Manager, to add this script to your website.
* Pixel
  1. After choosing an event on the 'Install Instructions' tab, select the Pixel option.
  2. If you have configured custom data fields, please use the indicated placeholders to inform the values.
  3. Click on <img src="../.gitbook/assets/image (49) (1).png" alt="copy button" data-size="line"> to copy the Pixel tag.&#x20;
  4. Add the Pixel tag to your website's code, on the page where the event will be tracked.
  5. You can also use a tag manager, like Google Tag Manager, to add this script to your website.
* Redirect
  1. After choosing an event on the 'Install Instructions' tab, select the Redirect option.
  2. Provide the URL to which the user should be redirected after the event is captured.
  3. If you have configured custom data fields, please use the indicated placeholders to inform the values.
  4. Click on <img src="../.gitbook/assets/image (49) (1).png" alt="copy button" data-size="line"> to copy the generated URL and use it as it was the URL you provided before.

### Tracker's Metrics Tab

The metrics tab allows you to visualize how your trackers, events, and actions are performing. On the metrics tab of the trackers' page, it´s possible to filter the data that is displayed according to your preference, here are the available filters at the moment:

* "Group By": Select how you want to group the displayed data, by tracker or by event.
* "Visualization":  Select how you want to display your data, metric cards, or table.
* "Period": Select the period that contains the data you need.

The data collected by the trackers makes it possible to show dynamic customized ads to your target, without it, it's impossible to generate or show dynamic banners.

## Recommendation Models&#x20;

Recommendation models are used to fill up your dynamic banners with data about your products based on your catalogs and the tracked activity of your website.

### Creating a Recommendation Model

1. On the [BMS homepage](https://console.bluems.com/), click on Recommendation Models, in the CS2 section.
2. Click on <img src="../.gitbook/assets/image (50) (1).png" alt="Create recommendation model button " data-size="line"> to create a new recommendation model.
3. Set a Name and Tags for it.
4. Select the catalog from which the model will collect data and lead interactions.
5. Click on <img src="../.gitbook/assets/image (51) (1).png" alt="save button" data-size="line"> to save your changes.

If you stop using a recommendation model, we recommend disabling it instead of deleting it, as deleting a model also deletes the data collected by this recommendation model.

### Setting up a Source

Now that we've created our recommendation model, we need to set up some sources for it, there are 2 source types available, DMP trackers and Catalogs (CS2). Using DMP trackers as a source will relate your recommendation model to the data collected by the trackers installed on your website. The Catalogs (CS2) option will relate your recommendation model to your catalog data, establishing a product ranking. Below are the steps to set up a source based on the desired source type:

* DMP Trackers
  1. Select the recommendation models you want to use this source for.
  2. In the Configuration tab click on <img src="../.gitbook/assets/image (52) (1).png" alt="+ add button" data-size="line"> to add a new Source.
  3. Set a Name.
  4. Set a limit of catalog products from which data will be collected.
  5. Choose DMP Tracker as the source's type.
  6. Select the tracker from which you will collect the data.
  7. Select the event configured on the tracker from which you will collect data.
  8. Set the field containing your offer IDs.
  9. Click on <img src="../.gitbook/assets/image (53) (1).png" alt="save button" data-size="line"> to save your changes.
* CS2 Product Ranking
  1. Realize the steps 1-4 above.
  2. Choose CS2 Product Ranking.
  3. Select the action you want to use to rank products for this source.
  4. Inform the period in which metrics will be checked and collected.
  5. &#x20;Click on <img src="../.gitbook/assets/image (54) (1).png" alt="save button" data-size="line"> to save your changes.

Sources are used to bring your product data to your dynamic banner, you must have at least one source for each space available in your dynamic banner, each source fills up only one space at a time, so if you have more spaces than sources, some spaces will be empty on your dynamic banners. We also recommend setting up at least 3 sources per recommendation model.

## Creative Builder

Use the Creative Builder to create blueprints and builds that will help you to create your ads faster.

### Blueprints

Blueprints are models for creating ads quickly and efficiently. These pre-made models allow you to build ads that meet your business needs with ease.&#x20;

Built on web design languages, Blueprints can offer you the flexibility of creating dynamic banners. Even, if you are not familiar with web development languages, you can confidently use one of the pre-made Blueprints available.&#x20;

#### How to use Blueprints

At first, you will need to choose between creating a blueprint on your own or using an already existing blueprint.

* **Creating a blueprint model.**
  1. Locate and click on Blueprints on the [BMS homepage](https://console.bluems.com/).
  2. Click on <img src="../.gitbook/assets/image (24) (1) (1).png" alt="add blueprint button" data-size="line">.
  3. Set a Name for your Blueprint.
  4. Set tags to make it easier to find it later.
  5. Choose the availability according to your preference, selecting public will make your blueprint available for everyone using the BMS platform, and private makes it available only for you and those with access to your account.
  6. Select the desired banner sizes.
  7. Click on ![](<../.gitbook/assets/image (25) (1) (1).png>) to add a new parameter group and start coding your banner
  8. Feel free to use the given system parameters according to your needs.
  9. You can also use our Macros for better interaction with your ads' viewers.
* **Using an existing Blueprint model**
  1. Locate and click on Blueprints on the [BMS homepage](https://console.bluems.com/).
  2. Turn off the 'Owned' option, this will show you all the public Blueprints available at the moment.
  3. Choose the Blueprint according to your business needs between the options available.
  4. Click on ![](<../.gitbook/assets/image (26) (1) (1).png>) to duplicate the blueprint to your account.
  5. Click on ![](<../.gitbook/assets/image (27) (1) (1).png>) to start editing your copy of the blueprint, here you can make changes to the blueprint, adjusting it to better reflect your business needs.

### Builds

Create builds using your blueprint models, builds help you create dynamic banners showing products from your catalog, used for your retargeting campaigns.

#### Creating Dynamic Banners Using Builds

1. On the [BMS homepage](https://console.bluems.com/), locate and click on Builds
2. Click on <img src="../.gitbook/assets/image (62) (1).png" alt="create build button" data-size="line"> to start creating a new build.
3. Now set a Name for it, you can also set tags to make it easier to track it.
4. Choose your domain.
5. Now select a blueprint model.
6. Select the sizes for your banners. It's recommended to use sizes with equal proportions for each build, for example, use one build for vertical banners and then create another for horizontal banners, this will keep the proportions of the logos, images, and products shown.
7. Use the Parameters on the left side to set and customize your logos, images, product grids, and more.
8. As you change the parameters, you can see a live preview of how your banner will be shown to help you find the perfect adjustment for your business needs.
9. Flag the box "Send creatives for approval" and click on <img src="../.gitbook/assets/image (63) (1).png" alt="" data-size="line"> to save your build and send it for the Ad Exchanges review.

## Creative Groups

Group several creatives as a single unit to apply different weights and compare performance between variants, this comparison is known as A\B test and it's very useful to discover what kinds of creatives are more interesting to your audience.

### Creating a Creative Group

1. On the [BMS homepage](https://console.bluems.com/) click on Creative Groups, in the AdServing Section.
2. Click on <img src="../.gitbook/assets/image (64) (1).png" alt="add creative build button" data-size="line"> to create a new creative group.
3. Set a Name and Tags for it.
4. Select your domain.
5. Select the format of the creatives in the group.
6. Select the creatives that should be in this group. Click on <img src="../.gitbook/assets/image (66).png" alt="Add button" data-size="line"> to add more fields and select your creatives.
7. Set a weight for each creative you've added.
   * This weight should be used to define what creatives you want to be displayed more often to your target, the greater the weight of a creative, the more it will be displayed.&#x20;
8. You can get a preview of your group after finishing this setup,  click on <img src="../.gitbook/assets/image (65).png" alt="Preview group button" data-size="original"> to see the preview.
9. Click on ![save button](<../.gitbook/assets/image (67).png>) to save your changes.

## Ads

Here is where you create your ads using your creative groups and send them to the AdExchanages Review, you can also create rules to control how your ads will be delivered, and follow your ads' status and metrics.

### Creating an Ad

1. On the [BMS homepage](https://console.bluems.com/) click on Ads, in the AdServing section.
2. Click on <img src="../.gitbook/assets/image (68).png" alt="create add button" data-size="line"> to create your ad.
3. Name it and set tags for it.
4. Select your domain.
5. Choose a format for your ad.
6. Select the creative group you want to use.&#x20;
7. If you don't have a creative group or need a new one, you can quickly create one by clicking on <img src="../.gitbook/assets/image (69).png" alt="create a creative group button" data-size="original">.
8. Check the box to send your ad for review on all supported ad exchanges.
9. Click on ![Save button](<../.gitbook/assets/image (70).png>) to save your ad.

### Bulk Ads

You can use this option to create ads quickly and massively.

1. Click on <img src="../.gitbook/assets/image (71).png" alt="Create bulk ads button" data-size="line"> to start.
2. Set a Name and Tags for your ads.
3. Select your domain.
4. Inform the URL to where the ad should redirect to when clicked, parametrization is allowed (UTM, for example).
5. Click on <img src="../.gitbook/assets/image (55) (1).png" alt="" data-size="line"> to add your creatives' images according to the options below:
   * &#x20;Use Existing
     1. Select all the images you want between the ones you've already uploaded to the platform.
     2. Click on <img src="../.gitbook/assets/image (56) (1).png" alt="" data-size="line"> to confirm your selection.
   * Upload New
     1. Upload new images to the platform by dragging them to the box or clicking on <img src="../.gitbook/assets/image (57) (1).png" alt="" data-size="line"> and selecting them on your device storage.
     2. Click on <img src="../.gitbook/assets/image (56) (1).png" alt="" data-size="line"> to confirm your selection.
   * Use Web Adress (URL)
     1. Add one image URL per line.
     2. Click on <img src="../.gitbook/assets/image (56) (1).png" alt="" data-size="line"> to confirm your selection.
6. Flag the option to group creatives of the same format to be able to perform an A/B test.
7. Flag the option to send your ads to a review from the AdExchanges.
8. Click on <img src="../.gitbook/assets/image (58) (1).png" alt="" data-size="line"> to save your ads and send them to review.

### Rules

In this tab, you can set up rules for running your ads only in specific hours and days.&#x20;

#### Creating a Rule

1. Select the ad you want to set a rule for.
2. In the Rule tab click on <img src="../.gitbook/assets/image (59) (1).png" alt="" data-size="line"> to add a new rule.
3. Set a Name for it and select what Creative Group should be affected.
4. Switch the Scheduling option to "on"<img src="../.gitbook/assets/image (60) (1).png" alt="" data-size="original">.
5. Select the hours you want your ads to be displayed on each day. If there are some days you don't need this ad to run, unflag all the hours on these days, and it won't be running on these days.
6. Click on <img src="../.gitbook/assets/image (61) (1).png" alt="" data-size="line"> to save your rule.
7. The rules can be activated/deactivated any time you want, you can do this by switching the rule between on and off on the rules tab.

### AdExchange Reviews

In the Exchange Reviews tab, after creating your ad, select it to monitor whether AdExchanges will approve or reject your ads. In case of refusal, you can check the reason in the comments column. After making the necessary adjustments, you can resend the ads for a new review.

## Campaigns

This is where you'll find and be able to monitor your campaigns.

In this article, we're approaching the creation of retargeting campaigns, to see a complete description of every function on this page, please check our[ campaigns' documentation](../product-documentation/demand-side-platform-dsp/).&#x20;

### Creating a Campaign

1. On the BMS homepage, click on Campaigns, in the campaigns section.
2. Click on <img src="../.gitbook/assets/image (28) (1) (1).png" alt="" data-size="line"> to start creating your campaign.
3. Set a Name and tags for it.
4. Select your domain and time zone.
5. Set when the campaign should start and end.
6. Set your Bid price:
   * Fixed: This option will use the configured value to bid. Please insert your target CPM value here.
   * Variable: This option will optimize your bid's cost in a defined range, looking for the smallest bids possible. Insert the lowest and the highest value of your CPM.
7. Set the frequency cap, this is the number of times an ad of the same campaign will display to the same user.
8. Set how many bids you want to request for a second.
9. Click on <img src="../.gitbook/assets/image (29) (1) (1).png" alt="" data-size="line"> to save your campaign.

### Target

After creating your campaign, you'll need to set a target for it, we have some options to help you build your ideal target, including geographic location, language, domains' categories, domains, keywords, cookie pools, and AdExchanges. Our targets work on an 'AND' system, which means that every target added to a campaign will work with the others to bring you a more specific and qualified audience.

#### Creating a Target

1. Select the campaign that will receive this target.
2. On the Configuration tab, find the Target section and click on <img src="../.gitbook/assets/image (30) (1) (1).png" alt="" data-size="line"> to create your target.
3. Set a Name for your target.
4. On the Locations tab, you can set your target's location.
   * Geographies: Use this to include or exclude countries and regions where your campaign should be delivered.
   * Geofences: Define a location and the distance radius of where you want your campaign to be delivered.
5. On the Contents tab are some important settings for your target:
   * Languages: select the language of the websites where your ads will be displayed, you can also exclude languages that you don't want.
   * Categories: include specific categories so your ads will only appear on websites featuring content in those categories, you can also exclude categories, so your ads won't be shown on websites with content in those excluded categories.
   * Domains: include specific domains so your ads will only appear on those specified websites, you can also exclude domains so your ads won't be shown on those excluded websites.
   * URL Keywords: include or exclude URL keywords so you can refine where your ads appear based on the URL's content.
6. On the Devices tab, you can set parameters to your targets' devices:
   * Operational Systems: select operational systems so your ads will be displayed to users navigating the web on those systems, you can also exclude operational systems so your ads won't be shown to users on those excluded systems.
   * Browsers: select browsers so your ads will be displayed to users navigating the web through those browsers, you can also exclude browsers so your ads won't be shown to users on those excluded browsers.
   * Device Types: select device types so your ads will be displayed to users navigating the web on those devices, you can also exclude device types so your ads won't be shown to users on those excluded devices.
   * Visited URL Keywords: by defining Visited URL Keywords, you're tailoring which devices will see your ads based on their recent navigation history. We track the URL's that a device has accessed within the past 24 hours.
   * Visited Domains: By defining Visited Domains, you're tailoring which devices will see your ads based on their recent navigation history. We track the domains that a device has accessed within the past 24 hours.
   * Cookie Pools: select cookie pools so your ads will target only the users who have been added to those selected pools, you can also exclude certain cookie pools so your ads will not target users from those excluded pools. **This is a necessary setting for retargeting campaigns.**
7. On the Inventory tab, you can set your exchanges, viewability, and ads' position:
   * Exchanges: select ad exchanges to display your ads through those platforms, you can also exclude ad exchanges so your ads won't appear on those excluded platforms.
   * Position: select inventory positions to strategically place your ads for optimal visibility and engagement, you can also exclude positions to place your o ads on all non-excluded options.
   * Viewability: adjust the slider to set the minimum viewability threshold for ad slots. Your ads will only be matched with inventory positions where the viewability percentage is higher than the selected threshold.
8. Click on <img src="../.gitbook/assets/image (31) (1) (1).png" alt="" data-size="line"> to save your target.

### Budget

Here you set your campaign's daily budget in USD, you can also track how much of the budget has been spent already, how much you still have available, and the current budget target.

1. On the Configuration tab, in the budget section, inform your budget value in USD.
2. Click on <img src="../.gitbook/assets/image (31) (1) (1).png" alt="Save button" data-size="line"> to save your changes.

Now your retargeting campaign is ready to run, you only have to enable it and track how it goes on the metrics and real-time tabs. Here's an article on [how metrics work on the BMS platform](../product-documentation/demand-side-platform-dsp/campaigns.md#metrics).

{% hint style="info" %}
_Our bidding works by crossing the information of your configured campaign's settings and bid set, so you will be getting impressions based on your campaign's configuration only._
{% endhint %}
