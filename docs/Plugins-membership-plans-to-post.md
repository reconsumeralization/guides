# Memberships plans to post

With Subscriptions/Memberships you can charge daily, weekly, monthly or yearly subscription to your users to be able to post to your site.

### How to activate it?

Steps to follow:
1.  Login to your **Admin Panel** ->  **Configure**  ->  **Addons**.
2.  Find  **Subscriptions / Memberships** and activate the feature.
3.  Click  **Save**.


### Create Plans

1.  Login to your **Admin Panel** -> **Configure**  ->  **Addons** ->  **Subscriptions / Memberships** and click on configure.
2.  You can find the field **Plans** in the down part of the page.
3.  Click on **New plan**.
3.  Fill the fields.
4.  Click  **Submit**.

-   **Name:**  The name of the plan.
-   **Seoname:**  Friendly name for url.
-   **Description:**  Enter a description for the plan.
-   **Price:**  The price that users will be charged to subscribe to the plan.
-   **Days:**  The number of days that the plan renews.
-   **Amount Ads:**  The amount of ads that users can publish before their plan expires.
-   **Marketplace Fee:**  If  [Marketplace feature](Payment-set-up-marketplace-with-srtipe-connect.md)  is activated then seller is charged this fee instead of the one is configured.
-   **Status:**  If is checked, the plan is activated. Uncheck if you want to deactivate the plan.

![membership](https://raw.githubusercontent.com/yclas/guides/master/images/membership.png)

### Subscription Expire

With this option enabled, the user’s ads will expire and the profile becomes disabled. The ads and the user’s profile become available when the user renews or purchases their subscription plan.

To enable or disable this option, go to back to **Configure**  ->  **Addons** ->  **Subscriptions / Memberships**  ->  **Subscription Expire**. You can check the box to enable this feature.

### Give extra ad on mark as sold

With this option enabled, when users mark an ad as sold, they will have one extra ad on their membership.

![Mark as sold](https://raw.githubusercontent.com/yclas/guides/master/images/extra-ad-on-mark-as-sold.png)

To enable or disable this option, go to back to **Configure**  ->  **Addons** ->  **Subscriptions / Memberships**  ->  **Give extra ad on mark as sold**. You can check the box to enable this feature.

### How it works

When users click to  **Publish new ad**, they will be redirected to the pricing page where they can choose among the membership plans. Once they subscribe and pay, they will be able to post.

![pricing](https://raw.githubusercontent.com/yclas/guides/master/images/pricing.png)

Users can find information about their subscription at the bottom of the  **Edit profile**  page.

Once the subscription expires, an email will be sent to the user with a link to pay and renew his plan.

You can find information about all the users subscriptions when you go to your **Admin Panel** ->  **Addons**  ->  **Subscriptions**.

> **Note**: The amount of ads left for the subscriptions is discounted on every new published ad. Even if your users delete/deactivate any ad, it doesn't increase the amount of ads left. If there are no ads left, your user must upgrade to a plan with more ads.
>
> Logged in as an admin, you can always manually set the amount of ads left of your subscribers on Panel -> Subscriptions -> Edit -> Amount ads left.

### Recurring Membership Plans

Membership plans paid via  [Stripe payment gateway](Payment-set-up-marketplace-with-srtipe-connect.md)  with “Legacy Checkout” enabled and free plans are automatically renewed after the expiration date. Plans purchased with a different payment gateway need to be renewed by the user after the expiration date.

### Cancel Subscriptions

Users have the option to cancel their subscription renewal. In order to do that, they need to go to the user **Edit Profile** page and press a button called  **Cancel Subscription**.


<iframe width="100%" height="400px" src="https://www.youtube.com/embed/uKzO-8rEFWI" title="Yclas video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

