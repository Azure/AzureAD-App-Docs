##Prerequisites

You must have a valid tenant for [Google Apps for Work](https://www.google.com/work/apps/) or [Google Apps for Education](https://www.google.com/edu/products/productivity-tools/). You may use a free trial account for either service.

##Configure Google Apps for single sign on

To manually configure Google Apps to use Azure Active Directory for single sign-on, complete the following steps:

1.  First, ensure that the **Sign-on URL** is set appropriately in the Azure management portal. This is the URL for the Google Apps page that you want users to be redirected to upon sign-in, and should follow a format such as: https://mail.google.com/a/<yourdomain>

2.  Second, ensure a valid **SAML signing certificate** has been created in the Azure management portal.

3.  To begin configuring your Google Apps tenant to use Azure Active Directory as an identity provider, start by downloading the following certificate file , and saving it locally on your computer: [Download certificate](%metadata:CertificateDownloadUrl%)

4. Open a new tab in your browser, and sign into the [Google Apps Admin Console](http://admin.google.com/) using your administrator account.

6. Click **Security**. If you don't see the link, it may be hidden under the **More Controls** menu at the bottom of the screen. 

![Click Security.][10]

7. On the **Security** page, click **Set up single sign-on (SSO).** 

![Click SSO.][11]

8. Perform the following configuration changes: 

![Configure SSO][12] 

- Select **Setup SSO with third party identity provider**. 

- Enter the following value in the **Sign-in page URL** field in Google Apps: %metadata:SingleSignOnServiceUrl% 

- Enter the following value in the **Sign-out page URL** field in Google Apps: %metadata:SingleSignOutServiceUrl% 

- Enter the following value in the **Change password URL** field in Google Apps: https://account.activedirectory.windowsazure.com/changepassword.aspx

- In Google Apps, for the **Verification certificate**, upload the certificate that you downloaded in the step above. 

- Click **Save Changes**.

[10]: media/gapps-security.png
[11]: media/security-gapps.png
[12]: media/gapps-sso-config.png
