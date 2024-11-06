# Creative Groups

Creative Groups allow you to group several creatives as a single unit. You can then apply different weights to each and later check the performance of one against the others.

They are very useful if you wish to display several variants of the same banners while keeping a simple configuration for Ads. They are also how you can run [A/B tests](creative-groups.md#a-b-testing) to determine which creatives perform best.

## Managing Creative Groups

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Creative Group list</p></figcaption></figure>

### Creating a Creative Group

On the Creative Group page click on <img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt="Create Creative Group" data-size="line">.

Fill in the details:

<figure><img src="../../.gitbook/assets/image (143).png" alt=""><figcaption><p>Creating a Creative Group</p></figcaption></figure>

* Name - how you want to call this creative group;
* Tags - up to 5 labels that can be used to aid identification and searching;
* Domain - this is the primary domain that the creatives on this group will take the user when clicked;
* Type - the type of creative, can be any common IAB size like "Large Leaderboard (970x90)", "Banner (468x60)", etc.

Configure the creative group composition:

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Creative Group composition</p></figcaption></figure>

Select at least one creative to be a part of this group. To add more creatives, use the <img src="../../.gitbook/assets/add.png" alt="Add" data-size="line"> button. To remove an existing creative, use the <img src="../../.gitbook/assets/remove.png" alt="Remove" data-size="line"> button.

You can create a new creative directly from this editor by clicking on the <img src="../../.gitbook/assets/create.png" alt="Create" data-size="line"> button, or you can edit an existing creative by clicking on <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line">.

By default, the system will attribute equal weight to all creatives. If you wish to direct more traffic to one creative over another, simply adjust the weights column. The system will calculate the approximate ratio of impressions each one will have.

Click on the <img src="../../.gitbook/assets/preview group.png" alt="Preview Group" data-size="line"> button to see a preview of this group:

<figure><img src="../../.gitbook/assets/creative group preview.png" alt=""><figcaption><p>Creative Group editor screen</p></figcaption></figure>

After making all the necessary changes, click on <img src="../../.gitbook/assets/image (7) (7).png" alt="Save" data-size="line">.

### Editing a Creative Group

To edit a creative group use the <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> button on the creative group list. All fields are available for editing except the domain and type selectors.

<figure><img src="../../.gitbook/assets/image (6) (7).png" alt=""><figcaption><p>Editing a Creative Group</p></figcaption></figure>

Once you make the necessary changes to your creative group, click on <img src="../../.gitbook/assets/image (7) (7).png" alt="Save" data-size="line">.

### Checking the status of a Creative Group

In the Creative Group list, by hovering the mouse over the warning sign, you can check the status of your creative.

<figure><img src="../../.gitbook/assets/image (1) (2) (1).png" alt=""><figcaption><p>Issue being displayed for a creative group</p></figcaption></figure>

Once all issues are addressed the creative group will display a <img src="../../.gitbook/assets/image (8) (7).png" alt="Check" data-size="line">.

### Archiving and Unarchiving a Creative Group

Creative Groups that are not being used frequently can be archived by clicking on the <img src="../../.gitbook/assets/archive.png" alt="Archive" data-size="line"> button. Archiving a creative group does not prevent it from being used or displayed, just hides it from main view.

To see all archived creative groups, simply turn on the <img src="../../.gitbook/assets/archive filter.png" alt="Archived" data-size="line"> filter. You can unarchive <img src="../../.gitbook/assets/unarchive.png" alt="Unarchive" data-size="line"> a creative to move it to the main view.

### Deleting a Creative Group

You can delete a creative group by clicking on <img src="../../.gitbook/assets/delete.png" alt="Delete" data-size="line">. If the creative group is being used, you will be presented with a list of ads that will be affected. If you confirm the deletion, the ads will be modified to remove the deleted creative group from rotation.

<figure><img src="../../.gitbook/assets/image (9) (1) (1) (1).png" alt=""><figcaption><p>Delete confirmation screen showing that the creative group is being used.</p></figcaption></figure>

{% hint style="danger" %}
Attention! If you delete a creative group, all data related to that creative group, including previously collected metrics, will also be deleted, this action cannot be undone.
{% endhint %}

## Monitoring Creative Groups

### Metrics Tab

The metrics tab will display all metrics related to the selected creative groups or for the whole account if no creative groups are selected.

Learn more about the [Metrics tab](../ad-server/ad-server-metrics/creatives-metrics.md).

#### A/B testing

To check the performance of the creatives in a group, select the desired group on the list and then switch the metrics to be grouped by Creative instead of by Creative Group. You can then compare any of the available metrics between the creatives being tested in the group.

<figure><img src="../../.gitbook/assets/image (4) (1) (2).png" alt=""><figcaption><p>Checking metrics of an A/B creative test</p></figcaption></figure>

### Real Time Tab

The real time tab will display real time events related to the selected creative group.

Learn more about the [Real Time tab](../demand-side-platform-dsp/real-time-tab.md).
