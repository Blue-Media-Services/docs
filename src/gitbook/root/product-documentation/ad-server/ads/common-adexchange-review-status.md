---
description: Learn how the AdExchange Review Status works, how to identify and solve them.
---

# Common AdExchange Review Status

If your Ad is rejected during creation or by Google's daily checks, here are the most common errors you may be presented with and how to identify the problem.

Please note that sometimes AdExchange's rejection might not provide an accurate status for your Review. So, make sure to resend your ad for review to double-check the rejection status.



<figure><img src="../../../.gitbook/assets/image (8) (6).png" alt="" width="125"><figcaption><p>AdExchange Rejection</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

This document will present the main reasons for rejection by AdExchange, with examples so that you can make the necessary changes to your Ad:

* [ADULT CONTENT](common-adexchange-review-status.md#adult-content)
* [DESTINATION NOT CRAWLABLE](common-adexchange-review-status.md#destination-not-crawlable)
* [ONLINE GAMBLING](common-adexchange-review-status.md#online-gambling)
* [INAPPROPRIATE CONTENT](common-adexchange-review-status.md#inappropriate-content)
* [REMOVED BY GOOGLE](common-adexchange-review-status.md#removed-by-google)

## ADULT CONTENT

Explicit adult content is not allowed on the ad network. Some adult-oriented ads and landing pages are allowed but will be shown in limited scenarios based on user searches, user age, and local laws.

Below is a table where you can check if your creative presents any of the following examples. If it does, you will need to make adjustments to your creative before resubmitting the ad for review.



<table><thead><tr><th width="270">Category</th><th width="166">Restriction Level*</th><th>Example</th></tr></thead><tbody><tr><td>Partial Nudity</td><td>Moderate</td><td>Lower or outer curve of the female breast exposed, majority of buttocks exposed</td></tr><tr><td>Sexualized Theme Dating</td><td>Moderate</td><td>Affair dating, sexual fetish dating</td></tr><tr><td>Sexual Merchandise</td><td>Moderate</td><td>Sex toys, lubricants, aphrodisiacs, sexual enhancers, sexual fetish lingerie</td></tr><tr><td>Sexual Entertainment</td><td>Moderate</td><td>Strip clubs, adult movie festivals, sexually suggestive live streaming or live chat, sexually suggestive role playing games</td></tr><tr><td>Mature Cosmetic Procedures</td><td>Moderate</td><td>Female breast augmentation, penis enlargement surgery, vaginal laser rejuvenation, buttock implants, pubic hair grooming</td></tr><tr><td>Sexually Suggestive Elements and Theme</td><td>Moderate</td><td>Lewd or sexual language, images featuring legs spread open, touching covered intimate body parts, mimicking sexual positions or movements, dating for general audiences that includes more sexually suggestive imagery</td></tr><tr><td>Nudity</td><td>Strong</td><td>Visible genitalia, female breasts, or buttocks</td></tr><tr><td>Sexual Encounter Dating</td><td>Strong</td><td>Hook-up or fling dating, swinger dating sites</td></tr></tbody></table>

\***Restriction Level:**

* **Moderate** - Ads that feature or promote the following types of sexual content categories are moderately restricted. They will only serve based on the following conditions:
  * The user’s age, the local laws where the ad is being served, and the user’s Safe Search settings.
* **Strong** - Ads that feature or promote the following types of sexual content are strongly restricted. They will only serve based on the following conditions:
  * The user’s age, the local laws where the ad is being served, and the user’s Safe Search settings.
  * The user’s sexual content Search queries.

Once you receive a rejection for your ad, identify which example better suits your creative and make the necessary changes. After making the changes, resend the ad for review. If the changes made are correct, the ad will not be rejected.

Should you need any further information, check [here](https://support.google.com/adspolicy/answer/6023699?sjid=1157365488976502743-SA).

## DESTINATION NOT CRAWLABLE

Google requires that the destination and content of ads be accessible to the Google AdsBot web crawlers, ensuring that users are redirected to the correct destination after clicking on the ad.

In this scenario, the ads would be disapproved due to an untrackable destination.

Make sure Googlebot is allowed to crawl your landing page by checking your robots.txt file.

Below are some restrictions and errors you may have and how to identify them.



|            Error           |                                                       Context                                                       |                                                                                                                                                                              Example                                                                                                                                                                              |
| :------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|    Destination Mismatch    | The domain or domain extension in the display URL doesn’t match the final and mobile URLs where users are taken to. |                                                          Display URL: google.com and Final URL: example.com; Ad display URL: example.com and Keyword final URL: example.org; using the keyword insertion feature in the top-level or second-level domain of your display URL, such as "www.{keyword}.com"                                                         |
|  Destination Not Crawlable |                                  Destinations that are not crawlable by Google Ads                                  |                                                                                 Using exclusion files (such as "robots.txt") to restrict access to an entire site or to the majority of a site; restricting crawl capacity disproportionately to the number of ads being submitted                                                                                |
|   Destination Experience   |                 Destinations or content that are unnecessarily difficult or frustrating to navigate                 | Websites with pop-ups or interstitials that interfere with the user's ability to see the content requested; sites that disable or interfere with the browser's back button; websites that don't load quickly on most popular browsers and devices, or require download of an additional application to view the landing page (aside from common browser plug-ins) |
| Destination Not Accessible |                            Destinations that are not accessible in the targeted location                            |                                A site that displays a location based access limitation message in the targeted location (e.g. “This site is not accessible in your location”); a site that displays other messaging related to access limitations in the targeted location (e.g. “you do not have permission to access this page”)                                |

Check which situation your website fits into; you may need to consult your technical team to make the necessary changes to comply with the AdExchange's destination requirements.

You can also check [here](https://support.google.com/adspolicy/answer/6368661?sjid=8903565646488334037-SA#674) for a broader view of how to fix that issue.

## ONLINE GAMBLING

The promotion of online, real-money gambling or sites that contain or link to content related to online gambling is allowed with country-specific restrictions.

Social casino game ads are allowed on the Open Auction and Deals if they comply with the policies, which will be presented shortly, and if the advertiser has been certified Social casino game ads must target approved countries and should not appeal to minors. Check local regulations for the areas you want to target.

The promotion of social casino games, which are online simulated gambling games where there is no opportunity to win anything of value, such as money or prizes, is allowed.

However, the following are not allowed:

* Social casino game destinations that offer gambling or games where the opportunity exists to win real money or prizes based on the outcome of the game.
* Promotion of "real money gambling" destinations. This includes gambling-related advertisements that appear on your social casino game destination.

#### Gambling

Promoting ads for offline and online gambling is permitted. However, your ad must comply with the following:

|           Type          |                                                                                    Method                                                                                    |                                                                                                                                                                                                                                                           Examples                                                                                                                                                                                                                                                           |
| :---------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|     Offline Gambling    |                                                     Promotion of physical, real-money gambling activity or establishments                                                    |                                                                                                                                                                                                   "Brick and mortar casinos” in Las Vegas or Macau, entertainment events at casinos, streaming of offline poker tournaments                                                                                                                                                                                                  |
|     Online Gambling     |                           Promotion of online, real-money gambling; Promotion of sites that contain or link to content relating to online gambling                           | Online casinos or bookmakers, bingo or slots sites or apps, online lottery ticket or scratch card purchase, online sports betting, games played with virtual currencies or items that have real-world value, Promotional products such as vouchers or bonus codes; educational materials such as tutorials or e-books; software such as poker odds calculators; other gambling-related information including tips, odds, handicapping, and sports picks; aggregator or affiliate sites that promote gambling-related content |
| Online Non-Casino Games | Any internet-based game where money or other items of value are paid or wagered in exchange for the opportunity to win real money or prizes based on the outcome of the game |                                                                                                                                                                                                               Fantasy sports, online chess tournaments, or "match-three" video games played for money or prizes                                                                                                                                                                                                              |

Once you identify your method, you must comply with the rules of the country and get a certificate in order to display ads related to gambling.

Below, you can check the requirements for each country.

<figure><img src="../../../.gitbook/assets/image (170).png" alt="" width="529"><figcaption><p>Restrictions According to each Country.</p></figcaption></figure>

You will need the certificate for each country in which you are interested in publishing Ads.

For further information on how to apply for the certification, check [here](https://support.google.com/authorizedbuyers/answer/7450776).

## INAPPROPRIATE CONTENT

All ads and landing pages on Authorized Buyers must be designated as "family safe" to ensure they can potentially be shown to all appropriate audiences. It is necessary to identify how your creative fits into each category below.

|               Type              |                                                                                                                                                                       Content                                                                                                                                                                       |                                                                                                                                                                              Examples                                                                                                                                                                              |
| :-----------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Dangerous or Derogatory Content |                                                Content that incites hatred against, promotes discrimination of, or disparages an individual or group on the basis of their race or ethnic origin, religion, disability, age, nationality, veteran status, sexual orientation, gender, gender identity                                               |                                                                                             Content promoting hate groups or hate group paraphernalia; content that encourages others to believe that a person or group is inhuman, inferior, or worthy of being hated                                                                                             |
|    Sexually Explicit Content    | Text, image, audio, or video of graphic sexual acts intended to arouse, Content promoting underage, non-consensual, or other illegal sexual themes, whether simulated or real, Content promoting the creation or distribution of synthetic content that has been altered or generated to be sexually explicit or contain nudity as described above. | Hardcore pornography; sex acts such as genital, anal, and oral sex; masturbation; cartoon porn or hentai, incest, bestiality, necrophilia, lolita or teen-themed pornography, underage dating, sites or apps that claim to generate deepfake pornography, instructions on how to create deepfake pornography, endorsing or comparing deepfake pornography services |
|     Compensated Sexual Acts     |                                                                                                                                Content that may be interpreted as promoting a sexual act in exchange for compensation                                                                                                                               |                         Prostitution, companionship and escort services, intimate massage and similar services, cuddling sites; compensated dating or sexual arrangements where one participant is expected to provide money, gifts, financial support, mentorship or other valuable benefits to another participant such as ‘Sugar’ dating                        |
|        Mail-order brides        |                                                                                                                                                      Content promoting marriage to a foreigner                                                                                                                                                      |                                                                                                                                                  Mail-order brides, international marriage brokers, romance tours                                                                                                                                                  |
|  Adult Themes in Family Content |                                                     Content that is made to appear appropriate for a family audience but contains adult themes, including sex, violence, vulgarity, or other depictions of children or popular children’s characters, that are unsuitable for a general audience                                                    |                                                                                                                                                          Adult content targeting family content audience.                                                                                                                                                          |

If your creative matches any of the examples above, you will need to make the necessary changes accordingly. Make sure your creative does not present any of the above examples. After making the required changes, resend your ad for review.

For any further information you may need, check [here](https://support.google.com/adspolicy/answer/6015406?sjid=8903565646488334037-SA#360).

## REMOVED BY GOOGLE

This error may occur from time to time, based on the AdExchange review failing. You can try submitting the ad for review again. If the error persists, please contact our support team at support@bluems.com.
