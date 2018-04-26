## Prerequisites

To configure Azure AD integration with Adobe Sign, you need the following items:

- An Azure AD subscription
- A Adobe Sign single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Adobe Sign for single sign-on

1. In a different web browser window, log in to your Adobe Sign company site as an administrator.

2. In the SAML menu, click **Account Settings**, and then, click **SAML Settings**.
   
	![Account](./media/ic789520.png "Account")

3. In the **SAML Settings** section, perform the following steps:
  
	![SAML Settings](./media/ic789521.png "SAML Settings")
   
    a. As **SAML Mode**, select **SAML Mandatory**.
   
    b. Select **Allow Adobe sign Account Administrators to log in using their  Adobe Sign Credentials**.
   
    c. As **User Creation**, select **Automatically add users authenticated through SAML**.

	d. Paste **Azure AD SAML Entity ID** : %metadata:IssuerUri%, which you have copied from Azure portal into the **Entity ID/Issuer URL** textbox.
   	
	e. Paste **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%, which you have copied from Azure portal into the **Login URL/SSO Endpoint** textbox.
   
    f. Paste **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, which you have copied from Azure portal into the **Logout URL/SLO Endpoint** textbox.

	g. Open your **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** file in notepad, copy the content of it into your clipboard, and then paste it to the **IdP Certificate** textbox

	h. Click **Save Changes**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Adobe Sign with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-adobe-echosign-tutorial)
