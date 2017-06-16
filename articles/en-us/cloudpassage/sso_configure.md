## Prerequisites

To configure Azure AD integration with CloudPassage, you need the following items:

- An Azure AD subscription
- A CloudPassage single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring CloudPassage for single sign-on

1. In a different browser window, sign-on to your CloudPassage company site as administrator.

2. In the menu on the top, click **Settings**, and then click **Site Administration**. 
   
    ![Configure Single Sign-On][12]

3. Click the **Authentication Settings** tab. 
   
    ![Configure Single Sign-On][13]

4. In the **Single Sign-on Settings** section, perform the following steps: 
   
    ![Configure Single Sign-On][14]
	
	a. Paste **Azure AD SAML Entity ID** : %metadata:IssuerUri% into the **SAML issuer URL** textbox.
  
    b. Paste **Service Provider (SP) initiated endpoint** into the **SAML endpoint URL** textbox.
  
    c. Paste **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% into the **Logout landing page** textbox.
  
    d. Open your **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** in notepad, copy the content of downloaded certificate into your clipboard, and then paste it into the **x 509 certificate** textbox.
  
    e. Click **Save**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate CloudPassage with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-cloudpassage-tutorial)

[12]: ./media/tutorial_cloudpassage_07.png
[13]: ./media/tutorial_cloudpassage_08.png
[14]: ./media/tutorial_cloudpassage_09.png