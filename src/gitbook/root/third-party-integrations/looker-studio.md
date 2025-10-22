# Looker  Studio

Looker Studio is a business intelligence and data visualization platform that enables users to transform raw data into personalized reports. It integrates with multiple data sources, allowing users to create real-time dashboards for tracking performance and analyzing data.

{% hint style="warning" %}
_Attention! Before you continue, it is necessary to create an API Key with permission to read your account's metrics data, you can learn how to do it in our_ [_API Keys_](../product-documentation/identity-access-management-iam/api-keys.md) _article._
{% endhint %}

## Connecting BMS with Looker Studio

If you still don't have a BMS account, sign up [here](https://console.bluems.com/#signUp).

BMS has a partner connector in Looker Studio for the metrics API. This connector allows you to send data from your BMS campaigns to a customized report in Looker Studio. Below are the steps to configure BMS as a Data Source.

<figure><img src="../.gitbook/assets/image (4) (11).png" alt=""><figcaption><p>Looker Studio Homepage</p></figcaption></figure>

1. Access Looker Studio. You may need to create an account if you do not have one yet.
2. Go to the Data Sources tab, located just below the search bar.
3. Click on "+ Create New Data Source"
4. To rename your data source, click on the default name in the top-left corner of the page.
5.  Search for "BMS" in the search bar.\


    <figure><img src="../.gitbook/assets/image (1) (19).png" alt=""><figcaption><p>Finding BMS Connector</p></figcaption></figure>


6. Click on the BMS Monitoring to select it as a data source.
7.  Fill in with the correct parameters:\


    <figure><img src="../.gitbook/assets/image (2) (14).png" alt=""><figcaption><p>BMS Connector Parameters</p></figcaption></figure>



    * **BMS Account ID:** Enter the BMS account ID of the account you will connect to Looker Studio, using the format XXXX-XXXX-XXXX.
    * **BMS API Key:** Provide a BMS API Key secret code with permission to read the metrics data of your BMS account.
    * **Aggregation Period:** Define the default time interval for aggregating metric statistics when querying data by timestamps.
    * **Timezone Offset:** Set the UTC offset to determine the start of a day when grouping data by day.
    * **Allow "Aggregation Period" to be modified in reports:** Check this option if you want to allow the aggregation period to be modified in reports.
8. After filling out all the parameters correctly, click on "Connect" in the top right corner of the page to complete the connection.

## Additional Information

Now your BMS account metrics data is available as a data source for Looker Studio reports. You can use it to build customized reports that will provide valuable business insights. Here are some articles from Looker Studio to help you with this process:

* [Create a report](https://cloud.google.com/looker/docs/studio/create-a-report)
* [About connectors, data sources, and credentials](https://cloud.google.com/looker/docs/studio/about-connectors-data-sources-and-credentials)
* [Our Privacy Policy](https://bluems.com/privacy/home.html)
* [Our Terms of Use](https://console.bluems.com/assets/docs/signup-terms-and-conditions-20240404.pdf)
