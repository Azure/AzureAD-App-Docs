## Prerequisites

To configure Azure AD integration with QuickHelp, you need the following items:

- An Azure AD subscription
- A QuickHelp single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring QuickHelp for single sign-on

1. Sign-on to your QuickHelp company site as administrator.

2. In the menu on the top, click **Admin**.
   
    ![Configure Single Sign-On][21]

3. In the **QuickHelp Admin** menu, click **Settings**.
   
    ![Configure Single Sign-On][22]

4. Click **Authentication Settings**.

5. On the **Authentication Settings** page, perform the following steps
   
    ![Configure Single Sign-On][23]
   
    a. As **SSO Type**, select **WSFederation**.
   
    b. To upload your **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)**, click **Browse**, navigate to the file, end then click **Upload Metadata**.
   
    c. In the **Email** textbox, type `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress`.
   
    d. In the **First Name** textbox, `type http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname`.
   
    e. In the **Last Name** textbox, `type http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname`.
   
    f. In the **Action Bar**, click **Save**.

## Quick Reference

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate QuickHelp with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-quickhelp-tutorial)

<!--Image references-->


[21]: ./media/tutorial_quickhelp_05.png
[22]: ./media/tutorial_quickhelp_06.png
[23]: ./media/tutorial_quickhelp_07.png
