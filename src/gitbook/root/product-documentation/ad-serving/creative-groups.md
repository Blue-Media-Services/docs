# Creative Groups

A Creative Groups allow you to group several creatives as a single unit. You can then apply different weights to each and you can later check the performance of one against the others.

They are very useful if you wish to display several variants of the same banners while keeping a simple configuration for Ads. They are also how you can run [A/B tests](creative-groups.md#a-b-testing) to figure out what creatives perform the best.

## Managing Creative Groups

<figure><img src="../../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption><p>Creative Group list</p></figcaption></figure>

### Creating a Creative Group

1. In the Creative Group page click at the <img src="../../.gitbook/assets/create creative group.png" alt="Save" data-size="line"> button.
2.  Fill the details:

    <figure><img src="../../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption><p>Creative Group editor screen</p></figcaption></figure>

    * Name - how you want to call this creative group;
    * Tags - up to 5 labels that can be used to aid identification and searching;
    * Domain - this is the primary domain that the creatives on this group will take the user when clicked;
    * Type - the type of creative, can be any common IAB size like "Large Leaderboard (970x90)", "Banner (468x60)", etc.
3.  Configure the creative group composition:

    <figure><img src="../../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption><p>Creative Group composition</p></figcaption></figure>

    1. Select at least one creative to be a part of this group. To add more creatives use the <img src="../../.gitbook/assets/add.png" alt="Add" data-size="line"> button. To remove an existing creative use the <img src="../../.gitbook/assets/remove.png" alt="Remove" data-size="line"> button.
    2. You can create a new creative straight from this editor by clicking on the <img src="../../.gitbook/assets/create.png" alt="Create" data-size="line"> button or you can edit an existing creative by clicking on the <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> button.
    3. By default the system will attribute equal weight to all creatives. If you wish to direct more traffic to one creative over another, simply adjust the weights column. The system will calculate what is the approximate ratio of impressions that each one will have.
    4. Click on the ![Preview Group](<../../.gitbook/assets/preview group.png>) button to see a preview of this group:

    <figure><img src="../../.gitbook/assets/creative group preview.png" alt=""><figcaption><p>Creative Group editor screen</p></figcaption></figure>
4. If all is correct, click on the <img src="../../.gitbook/assets/save.png" alt="Save" data-size="line"> button.

### Editing a Creative Group

To edit a creative group use the <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> button on the creative group list. All fields are available for editing except the domain and type selectors.

### Checking the status of a Creative Group

On the Creative Group list you can check at a glance if there are any issues with your configuration. You can move the mouse over the warning sign to see a description of the issue.

<figure><img src="../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Issue being displayed for a creative group</p></figcaption></figure>

Once all issues are addressed the creative group will display a green check.

### Archiving and Unarchiving a Creative Group

Creative Groups that are not being used as often can be archived by clicking on the <img src="../../.gitbook/assets/archive.png" alt="Archive" data-size="line"> button. Archiving a creative group does not prevent it from being used or displayed, just hides it from main view.

To see all archived creative groups simply turn on the <img src="../../.gitbook/assets/archive filter.png" alt="Archived" data-size="line"> filter. You can unarchive <img src="../../.gitbook/assets/unarchive.png" alt="Unarchive" data-size="line"> a creative group to make it show again on the main list.

### Deleting a Creative Group

You can delete a creative group by clicking on <img src="../../.gitbook/assets/delete.png" alt="Delete" data-size="line">. If the creative group is being used, you will be presented with a list of ads that will be affected. If you confirm the deletion, the ads will be modified to remove the deleted creative group from rotation.

<figure><img src="../../.gitbook/assets/image (9) (1) (1).png" alt=""><figcaption><p>Delete confirmation screen showing that the creative group is being used.</p></figcaption></figure>

## Monitoring Creative Groups

### Metrics Tab

The metrics tab will display all metrics related to the selected creative groups or for the whole account if no creative groups are selected.

Learn more about the [metrics tab](../monitoring/metrics-tab.md).

#### A/B testing

To check the performance of the creatives in a group, select the desired group on the list and then switch the metrics to be grouped by Creative instead of by Creative Group. You can then compare any of the available metrics between the creatives being tested in the group.

<figure><img src="../../.gitbook/assets/image (4) (1) (2).png" alt=""><figcaption><p>Checking metrics of an A/B creative test</p></figcaption></figure>

### Real Time Tab

The real time tab will display real time events related to the selected creative group.

Learn more about the [real time tab](../monitoring/real-time-tab.md).
