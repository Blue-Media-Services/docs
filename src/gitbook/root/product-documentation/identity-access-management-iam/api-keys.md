---
description: Learn more about API Keys and how to integrate them with our platform.
---

# API Keys

The API Keys allow you to grant access to an API to your BMS account. This will make it easier to keep track of your metrics using an external platform. Some APIs, like Zapier, can be configured to create Ads based on Google Drive Files. When it comes to the APIs there is a lot we can do, and every API will have its particularities. However, the integration of these APIs with the BMS console is similar. This article aims to help you perform this integration.

## Managing API Keys

The API Keys are available on the permissions page, to access it click on your account's name on the top right corner, then click on Permissions, now on the menu at the left, click on API Keys.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-10-08 092211.png" alt=""><figcaption><p>API Keys List</p></figcaption></figure>

### Creating an API Key

It is possible to [Create New API Keys](api-keys.md#create-new-api-keys) and it is also possible to [Link an Existing API Key](api-keys.md#link-existing-api-key).

#### Create new API Keys

1. Click on <img src="../../.gitbook/assets/image (9).png" alt="" data-size="line"> to add an API Key
2.  Select Create API Key, then fill in the details.

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-08 100509.png" alt=""><figcaption><p>API Keys Editor</p></figcaption></figure>

    * Name: Set a name for your API Key.
    * Tags: Set tags for your organization.
    * Policies: Set access policies that limit what this API Key grants access to, click on <img src="../../.gitbook/assets/image (2) (1) (1).png" alt="" data-size="original"> to add your policies. Every policy has a name and a description of what it gives access to. You can also create the API Key without selecting a policy.

    <figure><img src="../../.gitbook/assets/image (146).png" alt=""><figcaption><p>Policies Selection Modal</p></figcaption></figure>

    * After selecting all the needed policies, click on <img src="../../.gitbook/assets/image (153).png" alt="" data-size="line"> to confirm your selection.
3. Click on <img src="../../.gitbook/assets/image (4) (1).png" alt="" data-size="line"> to save your API Key.

#### Link Existing API Key

This option allows you to link an existing API Key from another BMS account.&#x20;

{% hint style="info" %}
By linking an existing API Key, you will grant access to your account for the linked API Key users. Use policies to control what can be done through this API Key.
{% endhint %}

1. Click on <img src="../../.gitbook/assets/image (9).png" alt="" data-size="line"> to add an API Key.
2.  Select **Link existing API Key**, then fill in the details

    <figure><img src="../../.gitbook/assets/image (5) (10).png" alt=""><figcaption><p>Linking an Existing API</p></figcaption></figure>

    * API Key ID: Inform the API Key ID you want to link.
    * Policies: Set access policies that limit what this API Key grants access to by clicking on <img src="../../.gitbook/assets/image (2) (1) (1).png" alt="" data-size="original"> to add your policies. Every policy requires a name and a description of the access it provides. When linking API Keys, at least one policy must be selected.
    * After selecting all the necessary policies, click on <img src="../../.gitbook/assets/image (153).png" alt="" data-size="line"> to confirm your selection.
3. Click on <img src="../../.gitbook/assets/image (4) (1).png" alt="" data-size="line"> to save your API Key.

### Access Codes Tab

After creating the API Key, you need to generate an Access Code before you can start using it. If you select a linked API Key, this tab will remain disabled, as there is no need to create an access code. In such cases, you will use the Access Code of the linked API, which can be provided by its creator.

<figure><img src="../../.gitbook/assets/image (155).png" alt=""><figcaption><p>Access Codes Tab</p></figcaption></figure>

1. Select the API Key to which the access code needs to be created.
2.  Click on <img src="../../.gitbook/assets/image (156).png" alt="" data-size="line"> to create an access code for the selected API Key.\


    <figure><img src="../../.gitbook/assets/image (149).png" alt=""><figcaption><p>Access Code Creation</p></figcaption></figure>
3. Insert a description for your access code.
4. Click on <img src="../../.gitbook/assets/image (158).png" alt="" data-size="line"> to save your access code.
5.  Right after saving your changes, the access code secret will be displayed like this:

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-09 090427.png" alt=""><figcaption><p>Access Code Secret</p></figcaption></figure>
6. It's possible to copy the secret using the copy button, <img src="../../.gitbook/assets/image (419).png" alt="" data-size="original">, or download it into a '.txt' file.

You can create up to 2 access codes per API Key, each code is valid for 365 days, we strongly advise you to create a new code a few weeks before the actual code expires to guarantee that the services relying on this API Key don't stop.&#x20;

### How To Access BMS via API

To interact with BMS services programmatically, you need to include the Access Code generated in your API requests. Your access will be restricted to the specific APIs that your API key is authorized to use. You can include the Access Code in your requests using one of the following methods:

*   **In the Request Header**: Copy the "x-api-key", for this, use the button <img src="../../.gitbook/assets/image (151).png" alt="" data-size="original">. This will avoid typing errors, and paste it into the header of your requests.

    <figure><img src="../../.gitbook/assets/image (150).png" alt=""><figcaption><p>Acessing BMS via API - In the Request Header Method</p></figcaption></figure>
*   **In the Query String**: Add the Access Code to the URL as a query parameter apiKey. You can also use the copy button to avoid typing errors.

    <figure><img src="../../.gitbook/assets/image (152).png" alt=""><figcaption><p>Acessing BMS via API - In the Query String Method</p></figcaption></figure>

For a complete list of available BMS APIs, please refer to our [documentation](https://api.bluems.com/).

### Editing API Keys and Access Codes

All the API Keys details are available for edition by clicking on <img src="../../.gitbook/assets/image (420).png" alt="" data-size="line"> at the same row as the API Key you want to edit. After making your changes, click on <img src="../../.gitbook/assets/image (421).png" alt="" data-size="line">to save them.&#x20;

You can also delete an API Key by clicking on <img src="../../.gitbook/assets/image (422).png" alt="" data-size="original">, and then confirming the action on <img src="../../.gitbook/assets/image (423).png" alt="" data-size="line">. Be careful - this action cannot be undone. Keep in mind that any API relying on the deleted API Key will stop working.\
\
Regarding Access Codes, you can view the access code secret and download the credentials by clicking on <img src="../../.gitbook/assets/image (424).png" alt="" data-size="original"> at the same row as the access code you want to view. The access code description can also be edited as well by clicking on <img src="../../.gitbook/assets/image (420).png" alt="" data-size="line"> at the same row as the access code you wish to edit. Once you have finished making your changes, click on <img src="../../.gitbook/assets/image (421).png" alt="" data-size="line"> to save them.&#x20;

{% hint style="danger" %}
Attention! Be careful when deleting an access code, this action cannot be undone, and all services relying on this access code will stop working.
{% endhint %}

You can also delete access codes. This is useful in cases where the data may have been compromised. To do this, firts to disable the code by toggling the switch to the right of the access code off <img src="../../.gitbook/assets/image (425).png" alt="" data-size="original">, then clicking on <img src="../../.gitbook/assets/image (422).png" alt="" data-size="original"> at the same row as the access code you want to delete, and confirming by clicking on <img src="../../.gitbook/assets/image (423).png" alt="" data-size="line">.&#x20;
