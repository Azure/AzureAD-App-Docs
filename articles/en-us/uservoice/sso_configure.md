## Prerequisites

To configure Azure AD integration with UserVoice, you need the following items:

- An Azure AD subscription
- A UserVoice single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring UserVoice for single sign-on

1. In a different web browser window, log in to your UserVoice company site as an administrator.

2. In the toolbar on the top, click **Settings**, and then select **Web portal** from the menu.
   
    ![Settings](./media/IC777519.png "Settings")

3. On the **Web portal** tab, in the **User authentication** section, click **Edit** to open the **Edit User Authentication** dialog page
   
    ![Web portal](./media/IC777520.png "Web portal")

4. On the **Edit User Authentication** dialog page, perform the following steps:
   
    ![Edit user authentication](./media/IC777521.png "Edit user authentication")
   
    a. Click **Single Sign-On (SSO)**.
 
    b. Paste the **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% value into the **SSO Remote Sign-In** textbox.

    c. Paste the **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% value into the **SSO Remote Sign-Out textbox**.
 
    d. Copy the **Thumbprint** value from the exported certificate **[Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)**, and then paste it into the **Current certificate SHA1 fingerprint** textbox.  
      
    > [!TIP]
    > For more information, see [How to retrieve a certificate's thumbprint value](http://youtu.be/YKQF266SAxI)
 
    e. Click **Save authentication settings**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **[Download Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)**


## Additional Resources

* [How to integrate UserVoice with Azure Active Directory](active-directory-saas-uservoice-tutorial.md)
