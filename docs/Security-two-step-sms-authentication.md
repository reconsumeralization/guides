# Two-Step SMS Authentication


Keep your users secure with the two-step SMS authentication. Two-step authentication is a mechanism to double check that your identity is legitimate.

## How to enable and configure Two-step SMS Authentication:

1.  Register at  [Clickatell](https://www.clickatell.com/).
2.  On Clickatell dasboard, choose  **SMS integrations**.
3.  Click  **Activate Now**  and setup Billing Details. You can calculate the pricing  [here].(https://www.clickatell.com/pricing-and-coverage/message-pricing/#step-1)
4.  Now that the integration is activated, choose SMS integrations again and copy the  **API key**.
5.  In your website admin panel,  **Configure -> Integrations**, enable  **Clickatell**  and paste the API key into the  **Clickatell**  field.
6.  If your Clickatell integration is a two-way messaging type, paste your Two-way phone number into the  **Clickatell Phone Number**  field.
7.  Click  **Save**.

![clickatel](https://raw.githubusercontent.com/yclas/guides/master/images/clickatel.png)

Now customers that set a **phone number** in the profile will have the two-step sms authentication.

## Set regional country configuration

This option will make it easier for your customers to login or register to your site. Select the country your website is targeted to. This way, the country’s code will be the default country code in the phone field in the register, login and publish a new page.

Go to  **Settings**  ->  **General**  ->  **Regional**  ->  **Country**  and select the country your website is targeted to.

## How it works:

1.  A user registers on your website or posts an ad.
2.  A user account is created and the user goes to Edit Profile page and enters his phone number.
3.  After updating the profile details, the user will get a verification code by message on his mobile phone, which he will need to enter in the next page.
4.  Now the user is authenticated and the Two-step SMS authentication is enabled on his account.



## Register and login with phone number

### Register:

Users can choose to register with their email and password, or to choose to register with their phone number.

1.  A user visits your site and choose to register.
2.  We send them an SMS with a code.
3.  They enter the code, if it’s valid.
4.  We ask them for name and email.
5.  User is successfully registered.

### Login:

1.  Registered user visits your site and wants to login.
2.  He/She chooses to login with a phone number and enters his/her number.
3.  If the number is valid and a profile account with that phone number is found, we send them a code.
4.  The user enters the code.
5.  If the code is valid, the user is successfully logged in.




