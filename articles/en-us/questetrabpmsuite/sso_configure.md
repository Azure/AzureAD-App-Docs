## Prerequisites

To configure Azure AD integration with Questetra BPM Suite, you need the following items:

- An Azure AD subscription
- A Questetra BPM Suite single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Questetra BPM Suite for single sign-on

1. In a different web browser window, log into your **Questetra BPM Suite** company site as an administrator.

2. In the menu on the top, click **System Settings**. 
   
    ![Azure AD Single Sign-On][10]

3. To open the **SingleSignOnSAML** page, click **SSO (SAML)**. 
   
    ![Azure AD Single Sign-On][11]

4. On your **Questetra BPM Suite** company site, in the **SP Information** section, perform the following steps:

	a. Copy the **ACS URL**, and then paste it into the **Sign On URL** textbox in the **Questetra BPM Suite Domain and URLs** section from Azure portal.
	
	b. Copy the **Entity ID**, and then paste it into the **Identifier** textbox in the **Questetra BPM Suite Domain and URLs** section from Azure portal.

5. On your **Questetra BPM Suite** company site, perform the following steps: 
   
    ![Configure Single Sign-On][15]
   
	a. Select **Enable Single Sign-On**.
   
	b. In **Entity ID** textbox, paste the value of **Azure AD SAML Entity ID** : %metadata:IssuerUri% which you have copied from Azure portal.
	
	c. In **Sign-in page URL** textbox, paste the value of **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% which you have copied from Azure portal.
	
	d. In **Sign-out page URL** textbox, paste the value of **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% which you have copied from Azure portal.
	
	e. In the **NameID format** textbox, type `urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress`.

    f. Open your **[Downloaded Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)** in notepad downloaded from Azure portal, copy the content of it into your clipboard, and then paste it into the **Validation certificate** textbox. 

    g. Click **Save**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)**

## Additional Resources

* [How to integrate Questetra BPM Suite with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-questetra-bpm-suite-tutorial)

<!--Image references-->

[10]: ./media/questera_bpm_suite_03.png
[11]: ./media/questera_bpm_suite_04.png
[15]: ./media/questera_bpm_suite_08.png