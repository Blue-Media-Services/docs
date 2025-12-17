# Google Tag Manager

The tag managers are a free tool that makes it easier to add, manage, and update tracking codes (or “tags”) on your website. In this article, we are going to talk about one of them, the most popular and accessible, Google Tag Manager, or GTM, however, they all work similarly, so feel free to use the most convenient tag manager for you.

These are the topics covered in this article:

* [Installing GTM](google-tag-manager.md#installing-google-tag-manager)
* [Triggers](google-tag-manager.md#triggers)
* [Variables](google-tag-manager.md#variables)
* [Tags](google-tag-manager.md#tags)
* [Templates](google-tag-manager.md#templates)
* [Additional Information](google-tag-manager.md#additional-information)

## Installing Google Tag Manager

After creating an account on GTM, you must install the GTM code on your website pages. This code can be found on your container's homepage.

<figure><img src="../.gitbook/assets/Captura de tela 2024-11-05 105747.png" alt=""><figcaption><p>GTM Container Homepage</p></figcaption></figure>

Click on the container ID to open the GTM installation instructions. There are two snippets of code that must be installed on your website: the first goes into the `<head>`, and the second into the `<body>.`

<figure><img src="../.gitbook/assets/image (808).png" alt=""><figcaption><p>GTM Install Instructions</p></figcaption></figure>

After installing the GTM codes, you will be able to test your website to ensure the installation was done correctly.

## Triggers

Setting up triggers is crucial for monitoring specific actions or events on your website. Triggers determine when and where your tags should activate, enabling you to manage the data collected for each user interaction.

You can set up triggers on the Triggers page or while creating or editing a tag.

<figure><img src="../.gitbook/assets/image (809).png" alt=""><figcaption><p>Triggers Page</p></figcaption></figure>

GTM provides several types of triggers to capture different user actions. Here are the most commonly used ones in e-commerce tracking:

1. **Page View**: Activates when a page loads.
2. **Click**: Activates when a specific element on a page is clicked, such as an "Add to Cart" button.
3. **Form Submission**: Activates when a form on the page is submitted.
4. **Custom Event**: Activates based on custom JavaScript events, which are useful for complex interactions that don't have direct GTM triggers.
5. **DOM Ready**: Activates when the HTML for the page is loaded (before images and other media).

You can learn more about all the trigger types in this GTM [article](https://support.google.com/tagmanager/topic/7679108?sjid=9288738402311135972-SA).

### Setting up Triggers

Now, let's look at some examples to help you understand how to set up triggers:

_**Example 1:**_ _Setting Up an Add-to-Cart Trigger_

**Goal**: Activate a tag when a user clicks the "Add to Cart" button.

1. Identify the Button's CSS Selector or ID:
   * Right-click on the "Add to Cart" button on your website and select "**Inspect**." Find the unique CSS selector, ID, or class for the button (like `.example` or `#example`).
2.  Create the Trigger in GTM:

    <figure><img src="../.gitbook/assets/image (820).png" alt=""><figcaption><p>Trigger Configuration</p></figcaption></figure>

    * Click on <img src="../.gitbook/assets/image (810).png" alt="" data-size="line"> and then <img src="../.gitbook/assets/image (811).png" alt="" data-size="original"> to start setting up your trigger.
    * Select Click - All Elements if the button isn’t a link, or Click - Just Links if it’s a link.
    * Under Trigger Type, choose Some Clicks.
    * Set the conditions to match the button’s selector or ID. For instance:
      * Click Element > CSS Selector > `.example`.
    * Save the trigger and name it something descriptive, like **Add to Cart Click Trigger**.
3. Assign Trigger to a Tag:
   * Attach this trigger to the **Add to Cart** tag you created, so it only fires when this button is clicked.

_**Example 2:** Setting Up a Purchase Trigger_

**Goal**: Activate a tag when a user completes a purchase (typically on a "Thank You" or "Order Confirmation" page).

1. Use the Thank You Page URL:
   * Find the unique URL or URL pattern of the order confirmation page (e.g., `/thank-you` or `/order-confirmation`).
2.  Create a Page View Trigger:

    <figure><img src="../.gitbook/assets/image (821).png" alt=""><figcaption><p>Trigger Configuration</p></figcaption></figure>

    * Click on <img src="../.gitbook/assets/image (810).png" alt="" data-size="line"> and then <img src="../.gitbook/assets/image (811).png" alt="" data-size="original"> to start setting up your trigger.
    * Choose Page View as the trigger type.
    * Select Some Page Views.
    * Set the condition to match the Thank You page URL:
      * Page Path > contains > `/thank-you`.
    * Save the trigger as Purchase Confirmation Trigger.
3. Attach Trigger to Purchase Tag:
   * Assign this trigger to your Product Ordered tag to track completed purchases.

_**Example 3:** Using a Custom Event Trigger for Advanced Actions_

**Goal**: Activate a tag for actions that don't match standard triggers, like custom JavaScript events.

1. **I**mplement a Custom Event:
   *   If your e-commerce platform or developer can add custom JavaScript events, you can use a JavaScript `dataLayer.push` event. For example:

       ```javascript
       dataLayer.push({
         event: 'addToCart',
         productID: '12345',
         productName: 'Sample Product'
       });
       ```
2.  Create a Custom Event Trigger:

    <figure><img src="../.gitbook/assets/Captura de tela 2024-11-05 121903.png" alt=""><figcaption><p>Custom Event Trigger</p></figcaption></figure>

    * Click on <img src="../.gitbook/assets/image (810).png" alt="" data-size="line"> and then <img src="../.gitbook/assets/image (811).png" alt="" data-size="original"> to start setting up your trigger.
    * Select Custom Event as the trigger type.
    * In the Event Name field, enter the event name used in the `dataLayer.push`, like `addToCart`.
    * Save this trigger as an Add to Cart Custom Event Trigger.

## Variables

In GTM, variables are used to store information that can be utilized within tags, triggers, and other variables. They enhance the functionality of your tags and triggers by enabling them to adjust dynamically based on user actions or data present on the page.

<figure><img src="../.gitbook/assets/image (812).png" alt=""><figcaption><p>Variables Page</p></figcaption></figure>

### Understanding Variable Types

There are two variable types available in GTM:

1. **Built-in Variables**: GTM provides built-in variables for common actions, such as Page URL, Click URL, and Form ID. You can enable these directly in GTM.
2. **User-Defined Variables**: These are custom variables you create to capture specific data, such as a product ID or a button click class. User-defined variable types include:
   * **Data Layer Variables**: Retrieve values pushed into the `dataLayer` (e.g., a product ID from your site’s code).
   * **URL Variables**: Capture data from the page URL, , like parameters (e.g., parameters like `utm_campaign`).
   * **JavaScript Variables**: Retrieve values directly from JavaScript expressions (e.g., document object properties).
   * **Constant Variables**: Store fixed values (e.g., a static tracking ID used in multiple tags).

### Setting Up Variables

1. **Built-in Variables**
   * In the **Built-in Variables** section, click on <img src="../.gitbook/assets/image (900).png" alt="" data-size="line">.
   * Select the variables you want to enable by checking their boxes (e.g., Page URL, Click URL, Click Text, Form ID).
2.  **User-Defined Variables**

    *   **Example 1:** _Creating a Data Layer Variable_

        Data Layer Variables pull data that has been pushed to the `dataLayer`. This is useful when tracking specific actions or values, like a product ID or category.

        1.  **Push Data to the Data Layer** (if not already done):\
            On your site, make sure the necessary data is being pushed to the `dataLayer`. Here’s an example for a product page:

            ```javascript
            dataLayer.push({
                event: 'productViewed',
                productID: '12345'  // Unique identifier for the product
            });
            ```
        2.  **Create the Data Layer Variable in GTM**:

            <figure><img src="../.gitbook/assets/image (901).png" alt=""><figcaption><p>Variable Configuration - Data Layer Example</p></figcaption></figure>

            * In the User-Defined Variables section, click on <img src="../.gitbook/assets/image (816).png" alt="" data-size="line">.
            * Select Variable Configuration and choose Data Layer Variable.
            * In Data Layer Variable Name, enter the name used in your data layer push (e.g., `productID`).
            * Optionally, set a default value if the variable is empty (e.g., `unknown`).
            * Name and save the variable (e.g., DL - Product ID).
        3. **Test**: Use GTM’s Preview mode to test that the variable correctly captures the product ID.
    * **Example 2:** _Creating a URL Variable_

    <figure><img src="../.gitbook/assets/image (382).png" alt=""><figcaption><p>Variable Configuration - URL Example</p></figcaption></figure>

URL Variables allow you to capture data from the URL of the page, such as tracking parameters (`utm_campaign`) or specific page paths.

1. In the User-Defined Variables section, click on <img src="../.gitbook/assets/image (816).png" alt="" data-size="line">.
2. Choose Variable Configuration and select URL.
3. In the Component Type dropdown, choose the part of the URL you need:
   * Page Path: Captures the path after the domain (e.g., `/products/shoes`).
   * Query: Captures specific URL parameters like `utm_campaign`.
4. If you choose Query, enter the Query Key (e.g., `utm_campaign`).
5. Save the variable with a descriptive name, like URL - UTM Campaign.

### Using Variables

After creating variables, you can use them to make tags and triggers more dynamic.

1. **In Tags**: When configuring a tag, you can insert variables by selecting the \{{\}} symbol or typing \{{variable name\}}. For example:
   * Use \{{GA Tracking ID\}} in a Google Analytics tag for the Tracking ID field.
   * Use \{{DL - Product ID\}} to dynamically pass the product ID in a conversion tag.
2. **In Triggers**: Variables can be used in triggers to specify activating conditions. For example:
   * Create a trigger to fire on pages where \{{URL - Page Path\}} contains /checkout

## Tags

Tags are snippets of code used to collect data and monitor user interactions for marketing and analytics platforms. Instead of manually inserting each tag into your site’s code, GTM serves as a central hub, allowing you to manage all your tags in one place.

<figure><img src="../.gitbook/assets/image (822).png" alt=""><figcaption><p>Tags Page</p></figcaption></figure>

### Creating Tags

There are many things you can accomplish using tags. GTM offers several types of tags. Here is an example of how to create a tag using BMS's pixel codes.

<figure><img src="../.gitbook/assets/image (825).png" alt=""><figcaption><p>Tag Configuration</p></figcaption></figure>

1. On the Tags Page click on <img src="../.gitbook/assets/image (823).png" alt="" data-size="line"> to add a new tag and then on <img src="../.gitbook/assets/image (827).png" alt="" data-size="line"> to start configuring it.
2. Select Custom HTML from the list.
3. On the HTML field, paste the pixel code you need to install, on the example, a product added to cart pixel was used.
4. Remember to replace the Offer ID with the product identifier variable used on your website or use a previously configured GTM variable linked to it. You can learn more about how the BMS OfferID works in our [Catalogs](../product-documentation/catalog-storage-service-cs2/catalogs.md#install-instructions) article.
5.  Select the triggers that will control when this tag will be activated.\\

    <figure><img src="../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>
6. Name and save your tag.
7. Click on <img src="../.gitbook/assets/image (830).png" alt="" data-size="line"> to access a preview of your page with the tags installed and debug them if necessary. (This step is optional)
8. Click on <img src="../.gitbook/assets/Captura de tela 2025-04-24 103600.png" alt="" data-size="line"> to submit your changes to the live version of your website.

## Templates

Alternatively, you can use our BMS Universal Tag template to install BMS components into your website easily. This single template contains most of our product tags, and we will discuss the available actions further.

### Configuring BMS Universal Tag

When creating a new tag, you will need to choose the type of your tag, this is where you will find our template after searching for it as "BMS Universal Tag".

<figure><img src="../.gitbook/assets/image (1092).png" alt=""><figcaption><p>Choose tag type - Searching for BMS Universal Tag</p></figcaption></figure>

After selecting this template, you will need to fill in some details according to the action you need to execute. These are some of the available actions:

* [Track Page Loaded](google-tag-manager.md#track-page-loaded)
* [Add User to a Cookie Pool](google-tag-manager.md#add-user-to-a-cookie-pool)
* [Record User Activity in a Tracker](google-tag-manager.md#record-user-activity-in-a-tracker)
* [Count Event in Catalog](google-tag-manager.md#count-event-in-a-catalog)
* [Tag Container](google-tag-manager.md#tag-container)

#### Track Page Loaded

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103042.png" alt=""><figcaption><p>Track Page Loaded</p></figcaption></figure>

When triggered, this action will execute the [Page Load Tracking Tag](../product-documentation/ad-server/page-load-tracking-tag.md). To configure it, you will need to fill in the following details:

* **BMS Account ID**: Your 12-digit BMS account number.

#### Add User to a Cookie Pool

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103323.png" alt=""><figcaption><p>Add User to a Cookie Pool</p></figcaption></figure>

When triggered, this action will add users to a [Cookie Pool](../product-documentation/data-management-platform-dmp/cookie-pools.md). To configure it, you will need to fill in the following details:

* **BMS Account ID**: Your 12-digit BMS account number.
* **Cookie Pool ID**: Insert your Cookie Pool ID; it is available when creating or editing a cookie pool at the cookie pools editor.

#### Record User Activity in a Tracker

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103424.png" alt=""><figcaption><p>Record User Activity in a Tracker</p></figcaption></figure>

When triggered, this action will execute your [Tracker's](../product-documentation/data-management-platform-dmp/trackers/) actions. To configure it, you will need to fill in the following details:

* **BMS Account ID**: Your 12-digit BMS account number.
* **Tracker ID**: Insert your Tracker ID; it is available when creating or editing a tracker at the trackers editor. You can also use a variable from your website that brings your Tracker ID when called.
* **Event ID**: Insert the variable you have identified as the Event ID you want to capture.
* **Custom Data**: If you have configured custom data fields in your BMS Tracker, add them here.

#### Count Event in a Catalog

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103516.png" alt=""><figcaption><p>Count Event in a Catalog Action</p></figcaption></figure>

When triggered, this action will load your [Catalog's](../product-documentation/catalog-storage-service-cs2/catalogs.md) pixel into your website. To configure it, you will need to fill in the following details:

* **BMS Account ID**: Your 12-digit BMS account number.
* **Event**: Select the event you want to capture from the drop-down menu.
* **Catalog ID**: You can either insert your catalog's ID or a variable from your website that brings the ID when called.
* **Product ID**: Insert a variable from your website that brings the product ID when called.

#### Include Tag Container

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-22 102738.png" alt=""><figcaption><p>Tag Container Action</p></figcaption></figure>

When triggered, this action will load a [Tag Container](google-tag-manager.md#tag-container) into your website. To configure it, you will need to fill in the following details:

* **BMS Account ID**: Your 12-digit BMS account number.
* **Tag Container ID**: Insert the BMS Tag Container ID.
* **Custom Data**: If you have configured custom data fields for this tag container, add them here.

## Additional Information

Each e-commerce site or website has its own particularities. To configure Google Tag Manager correctly, it is important to be aware of these details. You can learn more about some of these e-commerce platforms in the links below:

* [How to use GTM on Nuvemshop](https://atendimento.nuvemshop.com.br/pt_BR/12313-codigos-externos/como-instalar-google-tag-manager-gtm-na-nuvemshop)
* [How to use GTM on Shopfy](https://help.shopify.com/en/manual/promoting-marketing/pixels/custom-pixels/gtm-tutorial)
* [How to use GTM on Wix](https://support.wix.com/en/article/connecting-your-google-tag-manager-account-to-your-wix-site)

Check out these articles to learn more about how your website or e-commerce platform works, and the names they use for events, product identifiers, etc.
