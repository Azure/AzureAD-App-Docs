## Prerequisites

To configure Azure AD integration with Evidence.com, you need the following items:

- An Azure AD subscription
- A Evidence.com single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Evidence.com for single sign-on

1. In a separate web browser window, login to your Evidence.com tenant as an administrator and navigate to **Admin** Tab

2. Click on **Agency Single Sign On**

3. Select **SAML Based Single Sign On**

4. Copy the **Azure AD SAML Entity ID** : %metadata:IssuerUri%, **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% and **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% values shown in the Azure portal and to the corresponding fields in Evidence.com.

5. Open your **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** file in notepad, copy the content of it into your clipboard, and then paste it to the **Security Certificate** box. 

6. Save the configuration in Evidence.com.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Evidence.com with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-evidence-tutorial)
