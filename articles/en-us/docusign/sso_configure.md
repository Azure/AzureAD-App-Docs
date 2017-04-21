## Prerequisites

To configure Azure AD integration with Docusign, you need the following items:

- An Azure AD subscription
- A Docusign single-sign on enabled subscription

> [!Note]: 
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- You should not use your production environment, unless this is necessary.
- If you don't have an Azure AD trial environment, you can get an one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Docusign for single sign-on

1. In a different web browser window, log into your **DocuSign admin portal** as an administrator.
2. In the navigation menu on the left, click **Domains**.
   
    ![Configuring single sign-on][51]
3. On the right pane, click **Claim Domain**.
   
    ![Configuring single sign-on][52]
4. On the **Claim a domain** dialog, in the **Domain Name** textbox, type your company domain, and then click **Claim**. Make sure that you verify the domain and the status is active.
   
    ![Configuring single sign-on][53]
5. In menu on the left side, click **Identity Providers**  
   
    ![Configuring single sign-on][54]
6. In the right pane, click **Add Identity Provider**. 
   
	![Configuring single sign-on][55]

7. On the **Identity Provider Settings** page, perform the following steps:
   
	![Configuring single sign-on][56]

    a. In the **Name** textbox, type a unique name for your configuration. Please do not use spaces.

    b. Enter the **Azure AD SMAL Entity ID** : %metadata:IssuerUri% into the **Identity Provider Issuer** textbox.

    c. Enter **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% into the **Identity Provider Login URL** textbox.

    d. Enter **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% into the **Identity Provider Logout URL** textbox.

    e. Select **Sign AuthN Request**.

    f. As **Send AuthN request by**, select **POST**.

    g. As **Send logout request by**, select **POST**.
8. In the **Custom Attribute Mapping** section, choose the field you want to map with Azure AD Claim. In this example, the **emailaddress** claim is mapped with the value of **http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress**. This is the default claim name from Azure AD for email claim. 
   
	> [!NOTE]
	> Use the appropriate **User identifier** to map the user from Azure AD to Docusign user mapping. Select the proper Field and enter the appropriate value based on your organization settings.
	> 
	> 
   
	![Configuring single sign-on][57]
9. In the **Identity Provider Certificate** section, click **Add Certificate**, and then upload the certificate. **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** file which you can download from Quick Reference section.
   
	![Configuring single sign-on][58]
10. Click **Save**.
11. In the **Identity Providers** section, click **Actions**, and then click **Endpoints**.   
   
	![Configuring single sign-on][59]
 
12. On **DocuSign admin portal**, in the **View SAML 2.0 Endpoints** section perform, the following steps:
   
	![Configuring single sign-on][60]
   
	a. Copy the **Service Provider Issuer URL**, and then paste it into the **Identifier** textbox on **Docusign Domain and URLs** section of the Azure portal following the pattern: 'https://contoso.docusign.com/*'.
   
	b. Copy the **Service Provider Login URL**, and then paste into the **Sign On URL** textbox on **Docusign Domain and URLs** section of the Azure portal following the pattern: 'https://contoso.docusign.com/*'.

	![Configure Single Sign-On](./media/active-directory-saas-docusign-tutorial/tutorial_docusign_url.png)
	  
	c.  Click **Close**
    
## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SMAL Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**


<!--Image references-->

[1]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_01.png
[2]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_02.png
[3]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_03.png
[4]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_04.png
[51]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_21.png
[52]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_22.png
[53]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_23.png
[54]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_19.png
[55]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_20.png
[56]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_24.png
[57]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_25.png
[58]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_26.png
[59]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_27.png
[60]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_28.png
[61]: ./media/active-directory-saas-docusign-tutorial/tutorial_docusign_29.png
[100]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_100.png

[200]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_200.png
[201]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_201.png
[202]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_202.png
[203]: ./media/active-directory-saas-docusign-tutorial/tutorial_general_203.png

## Additional Resources

* [How to integrate Docusign with Azure Active Directory](active-directory-saas-docusign-tutorial.md)
* [How to configure user provisioning with Docusign](active-directory-saas-docusign-user-provisioning-tutorial.md)