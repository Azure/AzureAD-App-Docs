## Prerequisites

To configure Azure AD integration with Workday, you need the following items:

- An Azure AD subscription
- A Workday single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring Workday for single sign-on

1. In a different web browser window, sign in to your Workday company site as an administrator.

1. In the **Search box** search with the name **Edit Tenant Setup – Security** on the top left side of the home page.

    ![Edit Tenant Security](./media/ic782925.png "Edit Tenant Security")

1. In the **Redirection URLs** section, perform the following steps:

    ![Redirection URLs](./media/ic7829581.png "Redirection URLs")

    a. Click **Add Row**.

    b. In the **Login Redirect URL**, **Timeout Redirect URL** and **Mobile Redirect URL** textbox, paste the **Login URL** : %metadata:singleSignOnServiceUrl% which you have copied from the **Set up Workday** section of Azure portal.

    c. In the **Logout Redirect URL** textbox, paste the **Logout URL** : %metadata:singleSignOutServiceUrl% which you have copied from the **Set up Workday** section of Azure portal.

    d. In **Used for Environments** textbox, select the environment name.  

   > **Note:**
   > The value of the Environment attribute is tied to the value of the tenant URL:  
   > -If the domain name of the Workday tenant URL starts with impl for example: *https:\//impl.workday.com/\<tenant\>/login-saml2.flex*), the **Environment** attribute must be set to Implementation.  
   > -If the domain name starts with something else, you need to contact [Workday Client support team](https://www.workday.com/en-us/partners-services/services/support.html) to get the matching **Environment** value.

1. In the **SAML Setup** section, perform the following steps:

    ![SAML Setup](./media/ic782926.png "SAML Setup")

    a.  Select **Enable SAML Authentication**.

    b.  Click **Add Row**.

1. In the **SAML Identity Providers** section, perform the following steps:

    ![SAML Identity Providers](./media/ic7829271.png "SAML Identity Providers")

    a. In the **Identity Provider Name** textbox, type a provider name (for example: *SPInitiatedSSO*).

    b. In the Azure portal, on the **Set up Workday** section, copy the **Azure AD Identifier** value, and then paste it into the **Issuer** textbox.

    ![SAML Identity Providers](./media/ic7829272.png "SAML Identity Providers")

    c. In the Azure portal, on the **Set up Workday** section, copy the **Logout URL** value, and then paste it into the **Logout Response URL** textbox.

	d. In the Azure portal, on the **Set up Workday** section, copy the **Login URL** value, and then paste it into the **IdP SSO Service URL** textbox.

	e. In **Used for Environments** textbox, select the environment name.

    f. Click **Identity Provider Public Key Certificate**, and then click **Create**.

    ![Create](./media/ic782928.png "Create")

    g. Click **Create x509 Public Key**.

    ![Create](./media/ic782929.png "Create")

1. In the **View x509 Public Key** section, perform the following steps:

    ![View x509 Public Key](./media/ic782930.png "View x509 Public Key")

    a. In the **Name** textbox, type a name for your certificate (for example: *PPE\_SP*).

    b. In the **Valid From** textbox, type the valid from attribute value of your certificate.

    c.  In the **Valid To** textbox, type the valid to attribute value of your certificate.

    > **Note:**
    > You can get the valid from date and the valid to date from the downloaded certificate by double-clicking it.  The dates are listed under the **Details** tab.

    d.  Open your **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** in notepad, and then copy the content of it.

    e.  In the **Certificate** textbox, paste the content of your clipboard.

    f.  Click **OK**.

1. Perform the following steps:

    ![SSO configuration](./media/WorkdaySSOConfiguratio.png "SSO configuration")

    a.  In the **Service Provider ID** textbox, type **https://www.workday.com**.

    b. Select **Do Not Deflate SP-initiated Authentication Request**.

    c. As **Authentication Request Signature Method**, select **SHA256**.

    ![Authentication Request Signature Method](./media/WorkdaySSOConfiguration.png "Authentication Request Signature Method")

    d. Click **OK**.

    ![OK](./media/ic782933.png "OK")

    > **Note:**
    > Please ensure you set up single sign-on correctly. In case you enable single sign-on with incorrect setup, you may not be able to enter the application with your credentials and get locked out. In this situation, Workday provides a backup log-in url where users can sign-in using their normal username and password in the following format:[Your Workday URL]/login.flex?redirect=n

## Quick Reference

* **Login URL** : %metadata:singleSignOnServiceUrl%

* **Logout URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD Identifier** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Workday with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-tutorial)
