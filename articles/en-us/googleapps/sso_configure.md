## Prerequisites

To configure Azure AD integration with G Suite, you need the following items:

- An Azure AD subscription
- A G Suite single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

## Video tutorial

How to Enable Single Sign-On to G Suite in 2 Minutes:

> [!VIDEO https://channel9.msdn.com/Series/Azure-Active-Directory-Videos-Demos/Enable-single-sign-on-to-Google-Apps-in-2-minutes-with-Azure-AD/player]

## Frequently Asked Questions

1.	**Q: Does this integration support Google Cloud Platform SSO integration with Azure AD?**
	
	A: Yes. Google Cloud Platform and Google Apps share the same authentication platform. So to do the GCP integration you need to configure the SSO with Google Apps.


2. **Q: Are Chromebooks and other Chrome devices compatible with Azure AD single sign-on?**
   
    A: Yes, users are able to sign into their Chromebook devices using their Azure AD credentials. See this [G Suite support article](https://support.google.com/chrome/a/answer/6060880) for information on why users may get prompted for credentials twice.

3. **Q: If I enable single sign-on, will users be able to use their Azure AD credentials to sign into any Google product, such as Google Classroom, GMail, Google Drive, YouTube, and so on?**
   
    A: Yes, depending on [which G Suite](https://support.google.com/a/answer/182442?hl=en&ref_topic=1227583) you choose to enable or disable for your organization.

4. **Q: Can I enable single sign-on for only a subset of my G Suite users?**
   
    A: No, turning on single sign-on immediately requires all your G Suite users to authenticate with their Azure AD credentials. Because G Suite doesn't support having multiple identity providers, the identity provider for your G Suite environment can either be Azure AD or Google -- but not both at the same time.

5. **Q: If a user is signed in through Windows, are they automatically authenticate to G Suite without getting prompted for a password?**
   
    A: There are two options for enabling this scenario. First, users could sign into Windows 10 devices via [Azure Active Directory Join](active-directory-azureadjoin-overview.md). Alternatively, users could sign into Windows devices that are domain-joined to an on-premises Active Directory that has been enabled for single sign-on to Azure AD via an [Active Directory Federation Services (AD FS)](active-directory-aadconnect-user-signin.md) deployment. Both options require you to perform the steps in the following tutorial to enable single sign-on between Azure AD and G Suite.

### Configuring G Suite for single sign-on

1. Open a new tab in your browser, and sign into the [G Suite Admin Console](http://admin.google.com/) using your administrator account.

2. Click **Security**. If you don't see the link, it may be hidden under the **More Controls** menu at the bottom of the screen.
   
    ![Click Security.][10]

3. On the **Security** page, click **Set up single sign-on (SSO).**
   
    ![Click SSO.][11]

4. Perform the following configuration changes:
   
    ![Configure SSO][12]
   
    a. Select **Setup SSO with third-party identity provider**.

    b. In the **Sign-in page URL** field in G Suite, paste the value of **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl% which you have copied from Azure portal.

    c. In the **Sign-out page URL** field in G Suite, paste the value of **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl% which you have copied from Azure portal. 

    d. In the **Change password URL** field in G Suite, paste the value of **Change password URL** which you have copied from Azure portal. 

    e. In G Suite, for the **Verification certificate**, upload the **[Downloaded Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)** from Azure portal.

	f. Select **Use a domain specific issuer**.

    g. Click **Save Changes**.

## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL** : %metadata:singleSignOutServiceUrl%  

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**


[10]: ./media/gapps-security.png
[11]: ./media/security-gapps.png
[12]: ./media/gapps-sso-config.png

## Additional Resources

* [How to integrate G Suite with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-google-apps-tutorial)
* [How to configure user provisioning with Google Apps](https://docs.microsoft.com/azure/active-directory/active-directory-saas-google-apps-provisioning-tutorial)