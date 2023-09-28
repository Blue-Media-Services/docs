# Real Time Tab

Ad and Campaign resources have a dedicated real time monitoring tab that allows the customer to see what is being delivered in real time.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Real time tab showing ads being delivered and user interactions as they happen</p></figcaption></figure>

The events available are:

* Impressions\
  This event is registered any time a campaign wins the right to display an ad to the end user. This is the point where the media acquisition cost is charged.
* Deliveries\
  This event is registered when the end user's browser requests the ad content from our ad server. This is the point where the ad server cost is charged.
* Displays\
  This event is registered when the end user's browser loads and displays the ad in a page.
* Views\
  This event is registered when at least 50% of the ad body is shown on the screen for at least 1 second.
* Clicks\
  This event is registered when the end user clicks on the ad. For this event to be tracked you must be using the BMS Click Tracker which is enabled by default but can be disabled by editing the creative's HTML code.

For any event displayed on the list, you can click on the details button to see more:

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Event detail screen</p></figcaption></figure>

Here you can observe all the details for a particular event such as the user's geolocation, IP, browser and device type. The parameters for the bid, ad exchange and domain and those related to the particular campaign, target, ad, ad rule, creative group and creative alongside with a preview for the creative itself.