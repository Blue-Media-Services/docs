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

# Tag Container

This feature allows you to create a customized tag container to install multiple tags and scripts from a single piece of code.

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption><p>Tag Container List</p></figcaption></figure>

### Creating Tag Containers

Follow the steps below to create your Tag Container. This process will guide you through the necessary steps to set up a customized container that can hold multiple tags and scripts, simplifying the management and deployment of tracking codes across your website.

{% hint style="info" %}
We use cookie pools and trackers as script examples to explain this feature, but you can use any script or tag you need.
{% endhint %}

1.  Click on <img src="../../.gitbook/assets/image (2) (9).png" alt="" data-size="line"> to start creating your Tag Container.\


    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-01 114707.png" alt=""><figcaption><p>Tag Container Editor</p></figcaption></figure>
2. Fill in the details:
   * Name: Set a name for your tag container.
   * Tags: Set tags for your better organization.
   * Template: Paste the scripts and tags you need to include in your tag container. In the example shown, a BMS Cookie Pool script was used. Notice that the account ID ("acc") and Cookie Pool ID ("cpid") values were replaced by the placeholders "\{{acc\}}" and "\{{cpid\}}". This allows the tag container to be used dynamically. Similarly, a BMS tracker script was also added.
   * Available Parameters: The parameters will appear in this section based on your Sample Input. You can click on them to copy their references.
   * Sample Input: This is where you will provide a sample input for your tag container. In the example shown, there are four parameters configured in the sample input:
     * "e": Refers to the event that should be tracked using our tracker script.
     * "t": Refers to the tracker ID to be used.
     * "acc": Refers to the BMS account ID.
     * "cpid": Refers to the cookie pool ID.
   * Preview: This section shows how your tag container will look after you fill in the parameters.
3. After finishing your editions, click on <img src="../../.gitbook/assets/image (3).png" alt="" data-size="line"> to save your tag container.

### Installing your Tag Container

Follow the steps on the install instructions tab to correctly install your tag container.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Install Instructions Tab</p></figcaption></figure>

1. Copy the script using the copy button <img src="../../.gitbook/assets/image (5).png" alt="" data-size="line">.
2. Replace the parameters with the corresponding values.
3. Paste it into your website's code.

### Editing or Deleting Tag Containers

All the fields on the tag container editor are available for edition, click on <img src="../../.gitbook/assets/image (6).png" alt="" data-size="line"> to edit your tag container.

{% hint style="danger" %}
Attention! Be careful when deleting tag containers, this action cannot be undone and all the related data, including previously collected metrics, will also be deleted.
{% endhint %}

It is possible to delete tag containers, by clicking on <img src="../../.gitbook/assets/image (7).png" alt="" data-size="line"> at the same row as the tag container you need to delete, and then clicking on <img src="../../.gitbook/assets/image (8).png" alt="" data-size="line"> to confirm this action.&#x20;

Alternatively, you can archive tag containers to help with organization. This can be done by clicking on <img src="../../.gitbook/assets/image (9).png" alt="" data-size="line"> at the same row as the tag container you want to archive. To view archived tag containers, turn the 'Archived' switch on ![](<../../.gitbook/assets/image (10).png>), located right above the tag containers list. To unarchive a tag container, click on <img src="../../.gitbook/assets/image (11).png" alt="" data-size="line"> at the same row as the tag container you want to unarchive.
