---
description: Learn How our Real Time Tab works.
---

# Pestaña de Tiempo Real

Ad and Campaign resources have a dedicated real time monitoring tab that allows the customer to see what is being delivered in real time.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-30 090101.png" alt=""><figcaption><p>Real time tab showing ads being delivered and user interactions as they happen</p></figcaption></figure>

The events available are:

* <img src="../../.gitbook/assets/impression event.png" alt="Impression" data-size="line">\
  This event is registered any time a campaign wins the right to display an ad to the end user. This is the point where the media acquisition cost is charged.
* <img src="../../.gitbook/assets/delivered event.png" alt="Delivered" data-size="line">\
  This event is registered when the end user's browser requests the ad content from our ad server. This is the point where the ad server cost is charged.
* <img src="../../.gitbook/assets/displayed event.png" alt="Displayed" data-size="line">\
  This event is registered when the end user's browser loads and displays the ad on a page.
* <img src="../../.gitbook/assets/viewed event.png" alt="Viewed" data-size="line">\
  This event is registered when at least 50% of the ad body is shown on the screen for at least 1 second.
* <img src="../../.gitbook/assets/clicked event.png" alt="Clicked" data-size="line">\
  This event is registered when the end user clicks on the ad. For this event to be tracked you must be using the BMS Click Tracker which is enabled by default but can be disabled by editing the creative's HTML code.

{% hint style="info" %}
Please note that the "impression" event can only be tracked for Campaigns and Ads.

When checking real time events for Creatives or Creative Groups no "impression" event can be recorded. The Ad Rules are determined only at the time of Ad Delivery. This is the point where the final creative group is selected and from it, the final creative is chosen.
{% endhint %}

You can choose what events to see by toggling the selector:

<figure><img src="../../.gitbook/assets/image (145).png" alt=""><figcaption><p>Event filter</p></figcaption></figure>

For any event displayed on the list, you can click on the details button ![](<../../.gitbook/assets/image (538).png>) to see more:

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-30 090243.png" alt=""><figcaption><p>Event detail screen</p></figcaption></figure>

Here you can observe all the details for a particular event such as the user's geolocation, IP, browser and device type. The parameters for the bid, ad exchange and domain and those related to the particular campaign, target, ad, ad rule, creative group and creative alongside a preview for the creative itself.
