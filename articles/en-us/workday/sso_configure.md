## Prerequisites

To configure Azure AD integration with Workday, you need the following items:

- An Azure AD subscription
- A Workday single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Workday for single sign-on

1. In a different web browser window, log in to your Workday company site as an administrator.

2. Go to **Menu \> Workbench**.
   
    ![Workbench](./media/IC782923.png "Workbench")

3. Go to **Account Administration**.
   
    ![Account Administration](./media/IC782924.png "Account Administration")

4. Go to **Edit Tenant Setup – Security**.
   
    ![Edit Tenant Security](./media/IC782925.png "Edit Tenant Security")

5. In the **Redirection URLs** section, perform the following steps:
   
    ![Redirection URLs](./media/IC7829581.png "Redirection URLs")
   
    a. Click **Add Row**.
   
    b. In the **Login Redirect URL** textbox and the **Mobile Redirect URL** textbox, type the **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% you have entered on the **Workday Domain and URLs** section of the Azure portal.
   
    c. In the Azure portal, on the **Configure sign-on** window, copy the **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%, and then paste it into the **Logout Redirect URL** textbox.
   
    d.  In **Environment** textbox, type the environment name.  

    >**Note:**
    > The value of the Environment attribute is tied to the value of the tenant URL:  
    >-If the domain name of the Workday tenant URL starts with impl (for example, *https://impl.workday.com/\<tenant\>/login-saml2.htmld*), the **Environment** attribute must be set to Implementation.  
    >-If the domain name starts with something else, you need to contact [Workday Client support team](https://www.workday.com/en-us/partners-services/services/support.html) to get the matching **Environment** value.

6. In the **SAML Setup** section, perform the following steps:
   
    ![SAML Setup](./media/IC782926.png "SAML Setup")
   
    a.  Select **Enable SAML Authentication**.
   
    b.  Click **Add Row**.

7. In the SAML Identity Providers section, perform the following steps:
   
    ![SAML Identity Providers](./media/IC7829271.png "SAML Identity Providers")
   
    a. In the Identity Provider Name textbox, type a provider name (for example, *SPInitiatedSSO*).
   
    b. In the Azure portal, on the **Configure sign-on** window, copy the **Azure AD SMAL Entity ID**: %metadata:IssuerUri% value, and then paste it into the **Issuer** textbox.
   
    c. Select **Enable Workday Initiated Logout**.
   
    d. In the Azure portal, on the **Configure sign-on** window, copy the **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% value, and then paste it into the **Logout Request URL** textbox.

    e. Click **Identity Provider Public Key Certificate**, and then click **Create**. 

    ![Create](./media/IC782928.png "Create")

    f. Click **Create x509 Public Key**. 

    ![Create](./media/IC782929.png "Create")

8. In the **View x509 Public Key** section, perform the following steps: 
   
    ![View x509 Public Key](./media/IC782930.png "View x509 Public Key") 
   
    a. In the **Name** textbox, type a name for your certificate (for example, *PPE\_SP*).
   
    b. In the **Valid From** textbox, type the valid from attribute value of your certificate.
   
    c.  In the **Valid To** textbox, type the valid to attribute value of your certificate.
   
    > **Note:**
    > You can get the valid from date and the valid to date from the downloaded certificate by double-clicking it.  The dates are listed under the **Details** tab.
  
    d.  Open your base-64 encoded certificate in notepad, and then copy the content of it.
   
    e.  In the **Certificate** textbox, paste the content of your clipboard.
   
    f.  Click **OK**.

9. Perform the following steps: 
   
    ![SSO configuration](./media/WorkdaySSOConfiguratio.png "SSO configuration")
   
    a.  Enable the **x509 Private Key Pair**.
   
    b.  In the **Service Provider ID** textbox, type **http://www.workday.com**.
   
    c.  Select **Enable SP Initiated SAML Authentication**.
   
    d.  In the Azure portal, on the **Configure sign-on** window, copy the **Azure AD Single Sign-On Service URL: %metadata:singleSignOnServiceUrl% value, and then paste it into the **IdP SSO Service URL** textbox.
   
    e. Select **Do Not Deflate SP-initiated Authentication Request**.
   
    f. As **Authentication Request Signature Method**, select **SHA256**. 
   
    ![Authentication Request Signature Method](./media/WorkdaySSOConfiguration.png "Authentication Request Signature Method") 
   
    g. Click **OK**. 
   
    ![OK](./media/IC782933.png "OK")

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certificate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Workday with Azure Active Directory](active-directory-saas-workday-tutorial.md)
* [How to configure user provisioning with Workday](active-directory-saas-workday-user-provisioning-tutorial.md)
