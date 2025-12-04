---
description: Learn more about Blueprints and how to work with them!
---

# Blueprints

Blueprints are models for creating ads quickly and efficiently. These pre-made models allow you to code dynamic banners using web development languages, creating more engaging ads and improving the expected results.

Built on web design languages, Blueprints offer the flexibility of creating dynamic banners. Even if you are not familiar with web development languages, you can confidently use one of the pre-made Blueprints available.

## Managing Blueprints

<figure><img src="../../../../es-419/.gitbook/assets/Captura de tela 2024-12-05 072802.png" alt=""><figcaption><p>Blueprints List</p></figcaption></figure>

You will have some public blueprint models available for use, so even if you are not familiar with web development languages, you'll be able to create and use blueprints easily. You can also create a blueprint with your parameters by coding it; however, this option might require web development skills.

### **Creating a Blueprint**

Click on ![create blueprint](<../../../../es-419/.gitbook/assets/image (889).png>) to start creating your blueprint.

<figure><img src="../../../../es-419/.gitbook/assets/image (886).png" alt=""><figcaption><p>Blueprint Creation</p></figcaption></figure>

1. Fill in the Details:
   * Name: Set a name for your blueprint.
   * Tags: Set tags for your better organization.
   * Availability: Select if you want this blueprint to be public or private. Public blueprints will be available to everyone on BMS.
   * Generate Sizes: Select in which sizes this blueprint will build your creatives.
   *   Parameters: Click on ![](<../../../../es-419/.gitbook/assets/image (69) (2).png>) to create a new parameters group.\\

       <figure><img src="../../../../es-419/.gitbook/assets/image (327).png" alt=""><figcaption><p>Parameters Group Creator</p></figcaption></figure>

       * Name: Set a name for this parameters group.
       * Description: Set a description of the parameters group.
       * Click on ![save](<../../../../es-419/.gitbook/assets/image (13).png>) to save your parameter group.
2.  After creating the parameters group, you can begin coding your banner on the code box. Then, configure the parameters of your code to align with those in the parameter group. To add a new parameter to the group click on ![](<../../../../es-419/.gitbook/assets/image (310).png>) and fill in the details:

    <figure><img src="../../../../es-419/.gitbook/assets/image (335).png" alt=""><figcaption><p>Parameter Creator - Type Options</p></figcaption></figure>

    * Parameter ID: Use this identifier to insert the provided user value into your template.
    * Name: Set a name to your parameter.
    * Description: Set a description to your parameter.
    * Type: Select the data type of the input:
      *   **String**

          <figure><img src="../../../../es-419/.gitbook/assets/image (328).png" alt=""><figcaption><p>Parameter Editor - String Type</p></figcaption></figure>

          * Minimum Length: Set a minimum length for the input.
          * Maximum Length: Set a minimum length for the input.
          * Validation Regex: Insert the pattern used for the string validation.
          * Validation Message: This message is displayed to the user if the validation pattern doesn't match.
          * Select between the options:
            * Single-Line: Creates a field to enter a single line of text
            * Multi-Line: Creates a field that allows you to enter multiple lines of text.
          * Initial Value: This is the initial value the system will use when creating a new build.
      *   **Boolean**

          <figure><img src="../../../../es-419/.gitbook/assets/image (333).png" alt=""><figcaption><p>Parameter Editor - Boolean Type</p></figcaption></figure>

          * Initial Value: Check the box if the initial value is true, uncheck it if it's false.
      *   **Choice**

          <figure><img src="../../../../es-419/.gitbook/assets/image (334).png" alt=""><figcaption><p>Parameter Editor - Choice Type</p></figcaption></figure>

          * Label: Insert the label of your parameter.
          * Value: Insert the value associated with the label.
          * Add as many labels as you need by clicking on ![Add](<../../../../es-419/.gitbook/assets/image (891).png>).
          * Initial Value: Pick one of the configurated labels as the initial value.
      *   **Code**

          <figure><img src="../../../../es-419/.gitbook/assets/image (336).png" alt=""><figcaption><p>Parameter Editor - Code Type</p></figcaption></figure>

          * Type: Select the code language.
          * Code box: Insert your code into the code box.
      *   **Color**

          <figure><img src="../../../../es-419/.gitbook/assets/image (330).png" alt=""><figcaption><p>Parameter Editor - Color Type</p></figcaption></figure>

          * Initial Value: Insert the hex color code, or click on the color box to pick a color.
      *   **Number**

          <figure><img src="../../../../es-419/.gitbook/assets/image (332).png" alt=""><figcaption><p>Parameter Editor - Number Type</p></figcaption></figure>

          * Minimum: Insert the minimum value to be accepted.
          * Maximum: Insert the maximum value to be accepted.
          * Initial Value: Insert the initial value of the parameter.
      *   **Resource ID**

          <figure><img src="../../../../es-419/.gitbook/assets/image (331).png" alt=""><figcaption><p>Parameter Editor - Resource ID type</p></figcaption></figure>

          * Resource Type: Choose between a CS2 catalog or a CS2 Recommendation Model to use one of them as a resource for your banner.
          * Initial Value: Select the specific catalog or recommendation model you want to use for this parameter.
      *   **URL**

          <figure><img src="../../../../es-419/.gitbook/assets/image (329).png" alt=""><figcaption><p>Parameter Editor - URL Type</p></figcaption></figure>

          * Use Image Picker: Check this box to enable the image picker, in which you can pick images from your uploaded creatives, upload a new one if needed, or inform the image URL.
          * Initial Value: Insert the initial value for the image URL.
    * Click on ![save](<../../../../es-419/.gitbook/assets/image (13).png>) to save your parameter.
3. Continue adding parameter groups and parameters until your business needs are satisfied.
4. Use the available system parameters to customize your template:
   * Account ID: This option inserts on your template the account ID of the account where the build is created.
   * Banner Width: Insert the width in which the banner will be rendered.
   * Banner Height: Insert the height at which the banner will be rendered.
5. Use the available **macros** with your URLs, some of them are:
   * **Unescaped Click URL:** This macro will be replaced by BMS's unescaped click tracker URL. Use this option when BMS is the first click tracker on the chain.
   * **Escaped Click URL:** This macro will be replaced by BMS's escaped click tracker URL. Use this option when BMS is the second click tracker on the chain.
   * **Double-Escaped Click URL:** This macro will be replaced by BMS's double-escaped click tracker URL. Use this option when BMS is the third click tracker on the chain.
   * **Cache Buster:** This macro will be replaced by a random number that can be used for cache busting.
   * **Escaped Ad Context:** This macro will be replaced by an escaped JSON object containing data about the ad context, such as the campaign ID and users' data.
6. After finishing all your blueprint settings, click on <img src="../../../../es-419/.gitbook/assets/image (24) (1).png" alt="" data-size="line"> to save your blueprint.

### Using an Existing Blueprint

It's possible to use an existing blueprint as well. You can duplicate a blueprint you already have to reuse some of its parameters by clicking on <img src="../../../../es-419/.gitbook/assets/image (313).png" alt="" data-size="line"> at the same row as the blueprint you want to be duplicated. Additionally, you can use a public blueprint. Turn off the <img src="../../../../es-419/.gitbook/assets/image (314).png" alt="" data-size="line"> owned option, above the blueprints list, choose one of the available blueprints, and click on <img src="../../../../es-419/.gitbook/assets/image (313).png" alt="" data-size="line"> at the same row as the public blueprint you want to use. Turn on ![](<../../../../es-419/.gitbook/assets/image (316).png>)the owned option again, and then click on <img src="../../../../es-419/.gitbook/assets/image (318).png" alt="" data-size="line"> to edit the blueprint according to your business needs.

### Deleting Blueprints

You can delete or archive blueprints according to your needs. To archive blueprints, click on ![](<../../../../es-419/.gitbook/assets/image (319).png>) at the same row as the blueprint you want to archive. To view your archived blueprints, turn on the ![](<../../../../es-419/.gitbook/assets/image (316).png>) archived option above the list of blueprints.

{% hint style="danger" %}
Be careful when deleting blueprints, this action cannot be undone, and builds relying on the deleted blueprint will stop working, all the related data, including previously collected metrics, will also be deleted.
{% endhint %}

To delete blueprints click on ![](<../../../../es-419/.gitbook/assets/image (321).png>) at the same row as the blueprint you need to delete, then confirm the action by clicking on <img src="../../../../es-419/.gitbook/assets/image (322).png" alt="" data-size="line">.
