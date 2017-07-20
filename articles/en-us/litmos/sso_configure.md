## Prerequisites

To configure Azure AD integration with Litmos, you need the following items:

- An Azure AD subscription
- A Litmos single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Litmos for single sign-on

1. Sign-on to your Litmos company site [https://azureapptest.litmos.com/account/Login](`https://azureapptest.litmos.com/account/Login`) as an administrator.
   
    ![Azure AD Single Sign-On][21] 

2. In the navigation bar on the left side, click **Accounts**.
   
    ![Azure AD Single Sign-On][22] 

3. Click the **Integrations** tab.
   
    ![Azure AD Single Sign-On][23] 

4. On the **Integrations** tab, scroll down to **3rd Party Integrations**, and then click **SAML 2.0** tab.
   
    ![Azure AD Single Sign-On][24] 

5. Copy the value under **The SAML endpoint for litmos is:**.
   
    ![Azure AD Single Sign-On][26] 

6. In your **Litmos** application, perform the following steps:
    
     ![Azure AD Single Sign-On][25] 
     
	 a. Click **Enable SAML**.
    
	 b. Open **[Downloaded Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)** in notepad, copy the content of it into your clipboard, and then paste it to the **SAML X.509 Certificate** textbox.
	 
	 c. Click **Save Changes**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate Litmos with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-litmos-tutorial)

<!--Image references-->

[21]: ./media/tutorial_litmos_60.png
[22]: ./media/tutorial_litmos_61.png
[23]: ./media/tutorial_litmos_62.png
[24]: ./media/tutorial_litmos_63.png
[25]: ./media/tutorial_litmos_64.png
[26]: ./media/tutorial_litmos_65.png
