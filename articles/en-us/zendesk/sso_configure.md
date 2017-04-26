## Prerequisites

To configure Azure AD integration with Zendesk, you need the following items:

- An Azure AD subscription
- A Zendesk single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Zendesk for single sign-on

1. In a different web browser window, log in to your Zendesk company site as an administrator.

2. Click **Admin**.

3. In the left navigation pane, click **Settings**, and then click **Security**.
   
    ![Security](./media/IC773089.png "Security")

4. On the **Security** page, click the **Admin & Agents** tab.

5. Select **Single sign-on (SSO) and SAML**, and then select **SAML**.

6. In the Azure AD portal, on the ****Configure sign-on**** window, copy the **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% value from **Quick Reference** section, and then paste it into the **SAML SSO URL** textbox.

7. In the Azure AD portal, on the ****Configure sign-on**** window, copy the **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% value from **Quick Reference** section, and then paste it into the **Remote Logout URL** textbox.
    
    ![Single sign-on](./media/IC773090.png "Single sign-on")

8. Copy the **Thumbprint** value from the exported certificate, and then paste it into the **Certificate Fingerprint** textbox.**[Download Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)** from Quick Reference section.
    
    > [!TIP]
    > For more information, see. How to retrieve a certificate's thumbprint value](http://youtu.be/YKQF266SAxI)
   
9. Click **Save**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **[Download Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)**


## Additional Resources

* [How to integrate Zendesk with Azure Active Directory](active-directory-saas-zendesk-tutorial.md)
* [How to configure user provisioning with Zendesk](active-directory-saas-zendesk-user-provisioning-tutorial.md)
