# Ad Server

## Concepts

### Creatives

This is the smallest building block of our ad server. A creative represents the code that will be delivered to the end user when your ad is displayed.

You can provide the HTML code yourself or the platform can generate the HTML code for you if you give an image and link URL.

Creatives can be in one of 3 states: draft, in review, and approved. Any modification to a creative's content will put it in a draft where it won't be served to users. You can submit any changes for review and if everything is in accordance with our policies, the creative will be approved.

### Creative groups

Creative groups, as the name suggests, allow you to group several creatives while applying different weights to each.

This is most useful when running A/B tests with any number of creatives to measure which performs better.

### Ads

Ads are what the end user's browser requests from our Ad Server. They are composed of one or more rules where each rule specify a set of conditions that once met will direct the user to a particular creative group.

When the end user's browser makes the ad request, the creative group associated with the first rule that matches will be delivered. At this time, one of the creatives configured on the group will be randomly selected by weight and then delivered.

### Creative Builder

To simplify the creation of standardized creatives you can use Blueprints and Builds. These features can also be used to generate dynamic banners containing your products.

#### Blueprints

Blueprints define a base HTML code that can be dynamically generated based on user input. The parameters required for the generation can also be customized.

#### Builds

When you have a blueprint ready and wish to create creatives from it, you create a build. A build will record what creative sizes you want, the blueprint used, and all parameters. Once created, the build will generate all the creatives for you. You can at any moment alter any parameter and the creatives will be updated to reflect the change.
