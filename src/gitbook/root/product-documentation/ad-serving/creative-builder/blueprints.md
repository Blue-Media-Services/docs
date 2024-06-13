---
description: Learn more about Blueprints and how to work with them!
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

# Blueprints

Blueprints are models for creating ads quickly and efficiently. These pre-made models allow you to code dynamic banners using web development languages, creating more engaging ads and improving the expected results.

Built on web design languages, Blueprints offer the flexibility of creating dynamic banners. Even if you are not familiar with web development languages, you can confidently use one of the pre-made Blueprints available.&#x20;

## Managing Blueprints

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption><p>Blueprints List</p></figcaption></figure>

You will have some public blueprint models available for use, so even if you are not familiar with web development languages, you'll be able to create and use blueprints easily. You can also create a blueprint with your parameters by coding it; however, this option might require web development skills.

### **Creating a Blueprint**

1.  Click on <img src="../../../.gitbook/assets/image (24) (1) (1).png" alt="" data-size="line"> to create your blueprint.\


    <figure><img src="../../../.gitbook/assets/Captura de tela 2024-06-13 082435.png" alt=""><figcaption><p>Blueprint Editor</p></figcaption></figure>
2. Fill in the Details:
   * Name: Set a name for your blueprint.
   * Tags: Set tags for your better organization.
   * Availability: Select if you want this blueprint to be public or private. Public blueprints will be available to everyone on BMS.
   * Generate Sizes: Select in which sizes this blueprint will build your creatives.
   *   Parameters: Click on ![](<../../../.gitbook/assets/image (1) (10).png>) to create a new parameters group.\


       <figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption><p>Parameters Group Creator</p></figcaption></figure>

       * Name: Set a name for this parameters group.
       * Description: Set a description of the parameters group.
       * Click on <img src="../../../.gitbook/assets/image (2) (7).png" alt="" data-size="line"> to save your parameter group.
3.  After creating the parameters group, you can begin coding your banner on the code box. Then, configure the parameters of your code to align with those in the parameter group. To add a new parameter to the group click on ![](<../../../.gitbook/assets/image (3) (7).png>) and fill in the details:



    <figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption><p>Parameter Creator - Type Options</p></figcaption></figure>

    * Parameter ID: Use this identifier to insert the provided user value into your template.
    * Name: Set a name to your parameter.
    * Description: Set a description to your parameter.
    * Type: Select the data type of the input:
      *   **String**



          <figure><img src="../../../.gitbook/assets/image (21).png" alt=""><figcaption><p>Parameter Editor - String Type</p></figcaption></figure>

          * Minimum Length: Set a minimum length for the input.
          * Maximum Length:  Set a minimum length for the input.
          * Validation Regex: Insert the pattern used for the string validation.
          * Validation Message: This message is displayed to the user if the validation pattern doesn't match.
          * Select between the options:
            * Single-Line: Creates a field to enter a single line of text
            * Multi-Line: Creates a field that allows you to enter multiple lines of text.
          * Initial Value: This is the initial value the system will use when creating a new build.
      *   **Boolean**



          <figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption><p>Parameter Editor - Boolean Type</p></figcaption></figure>

          * Initial Value: Check the box if the initial value is true, uncheck it if it's false.
      *   **Choice**



          <figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption><p>Parameter Editor - Choice Type</p></figcaption></figure>

          * Label: Insert the label of your parameter.
          * Value: Insert the value associated with the label.
          * Add as many labels as you need by clicking on ![](<../../../.gitbook/assets/image (3) (7).png>).
          * Initial Value: Pick one of the configurated labels as the initial value.
      *   **Code**



          <figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption><p>Parameter Editor - Code Type</p></figcaption></figure>

          * Type: Select the code language.
          * Code box: Insert your code into the code box.
      *   **Color**



          <figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption><p>Parameter Editor - Color Type</p></figcaption></figure>

          * Initial Value: Insert the hex color code, or click on the color box to pick a color.
      *   **Number**

          <figure><img src="../../../.gitbook/assets/image (25).png" alt=""><figcaption><p>Parameter Editor - Number Type</p></figcaption></figure>

          * Minimum: Insert the minimum value to be accepted.
          * Maximum: Insert the maximum value to be accepted.
          * Initial Value: Insert the initial value of the parameter.
      *   **Resource ID**



          <figure><img src="../../../.gitbook/assets/image (24).png" alt=""><figcaption><p>Parameter Editor - Resource ID type</p></figcaption></figure>

          * Resource Type:  Choose between a CS2 catalog or a CS2 Recommendation Model to use one of them as a resource for your banner.
          * Initial Value: Select the specific catalog or recommendation model you want to use for this parameter.
      *   **URL**



          <figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption><p>Parameter Editor - URL Type</p></figcaption></figure>

          * Use Image Picker: Check this box to enable the image picker, in which you can pick images from your uploaded creatives, upload a new one if needed, or inform the image URL.
          * Initial Value: Insert the initial value for the image URL.
    * Click on <img src="../../../.gitbook/assets/image (2) (7).png" alt="" data-size="line"> to save your parameter.
4. Continue adding parameter groups and parameters until your business needs are satisfied.&#x20;
5. Use the available system parameters to customize your template:
   * Account ID: This option inserts on your template the account ID of the account where the build is created.
   * Banner Width: Insert the width in which the banner will be rendered.
   * Banner Height: Insert the height at which the banner will be rendered.
6. Use the available macros with your URLs:
   * Unescaped Click URL: This macro will be replaced by BMS's unescaped click tracker URL. Use this option when BMS is the first click tracker on the chain.
   * Escaped Click URL:  This macro will be replaced by BMS's escaped click tracker URL. Use this option when BMS is the second click tracker on the chain.
   * Double-Escaped Click URL: This macro will be replaced by BMS's double-escaped click tracker URL. Use this option when BMS is the third click tracker on the chain.
   * Cache Buster: This macro will be replaced by a random number that can be used for cache busting.
   * Escaped Ad Context: This macro will be replaced by an escaped JSON object containing data about the ad context, such as the campaign ID and users' data.
7. After finishing all your blueprint settings, click on <img src="../../../.gitbook/assets/image (2) (7).png" alt="" data-size="line"> to save your blueprint.

### Using an Existing Blueprint

It's possible to use an existing blueprint as well. You can duplicate a blueprint you already have to reuse some of its parameters by clicking on <img src="../../../.gitbook/assets/image (6) (7).png" alt="" data-size="line"> at the same row as the blueprint you want to be duplicated. Additionally, you can use a public blueprint. Turn off the <img src="../../../.gitbook/assets/image (7) (7).png" alt="" data-size="line"> owned option, above the blueprints list, choose one of the available blueprints, and click on <img src="../../../.gitbook/assets/image (6) (7).png" alt="" data-size="line"> at the same row as the public blueprint you want to use. Turn on  ![](<../../../.gitbook/assets/image (10).png>)the owned option again, and then click on <img src="../../../.gitbook/assets/image (11).png" alt="" data-size="line"> to edit the blueprint according to your business needs.

### Deleting Blueprints

You can delete or archive blueprints according to your needs. To archive blueprints, click on ![](<../../../.gitbook/assets/image (12).png>) at the same row as the blueprint you want to archived. To view your archived blueprints, turn on the ![](<../../../.gitbook/assets/image (10).png>) archived option above the list of blueprints.

{% hint style="danger" %}
Be careful when deleting blueprints, this action cannot be undone, and builds relying on the deleted blueprint will stop working.
{% endhint %}

To delete blueprints click on ![](<../../../.gitbook/assets/image (14).png>) at the same row as the blueprint you need to delete, then confirm the action by clicking on <img src="../../../.gitbook/assets/image (15).png" alt="" data-size="line">.
