## Prerequisites

To configure Azure AD integration with Promapp, you need the following items:

- An Azure AD subscription
- A Promapp single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Promapp for single sign-on

1. Sign-on to your Promapp company site as administrator. 

2. In the menu on the top, click **Admin**. 
   
    ![Azure AD Single Sign-On][12]

3. Click **Configure**. 
   
    ![Azure AD Single Sign-On][13]

4. On the **Security** dialog, perform the following steps:
   
    ![Azure AD Single Sign-On][14]
	
	a. Paste **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%, which you have copied from the Azure portal into the **SSO-Login URL** textbox.
	
	b. As **SSO - Single Sign-on Mode**, select **Optional**, and then click **Save**.

	c. Open the **[Downloaded Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)** in notepad, copy the certificate content without the first line (-----BEGIN CERTIFICATE-----) and the last line (-----END CERTIFICATE-----), paste it into the **SSO-x.509 Certificate** textbox, and then click **Save**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate (Base64 encoded)](%metadata:certificateDownloadBase64Url%)**

## Additional Resources

* [How to integrate Promapp with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-promapp-tutorial)

<!--Image references-->

[12]: ./media/tutorial_promapp_05.png
[13]: ./media/tutorial_promapp_06.png
[14]: ./media/tutorial_promapp_07.png
