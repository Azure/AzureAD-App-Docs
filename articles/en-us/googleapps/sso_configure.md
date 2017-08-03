## Prerequisites

To configure Azure AD integration with Google Apps, you need the following items:

- An Azure AD subscription
- A Google Apps single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

## Video tutorial
How to Enable Single Sign-On to Google Apps in 2 Minutes:

> [!VIDEO https://channel9.msdn.com/Series/Azure-Active-Directory-Videos-Demos/Enable-single-sign-on-to-Google-Apps-in-2-minutes-with-Azure-AD/player]
 
## Frequently Asked Questions
1. **Q: Are Chromebooks and other Chrome devices compatible with Azure AD single sign-on?**
   
    A: Yes, users are able to sign into their Chromebook devices using their Azure AD credentials. See this [Google Apps support article](https://support.google.com/chrome/a/answer/6060880) for information on why users may get prompted for credentials twice.
2. **Q: If I enable single sign-on, are users be able to use their Azure AD credentials to sign into any Google product, such as Google Classroom, GMail, Google Drive, YouTube, etch?**
   
    A: Yes, depending on [which Google apps](https://support.google.com/a/answer/182442?hl=en&ref_topic=1227583) you choose to enable or disable for your organization.
3. **Q: Can I enable single sign-on for only a subset of my Google Apps users?**
   
    A: No, turning on single sign-on immediately requires all your Google Apps users to authenticate with their Azure AD credentials. Because Google Apps doesn't support having multiple identity providers, the identity provider for your Google Apps environment can either be Azure AD or Google -- but not both at the same time.
4. **Q: If a user is signed in through Windows, are they automatically authenticate to Google Apps without getting prompted for a password?**
   
    A: There are two options for enabling this scenario. First, users could sign into Windows 10 devices via [Azure Active Directory Join](active-directory-azureadjoin-overview.md). Alternatively, users could sign into Windows devices that are domain-joined to an on-premises Active Directory that has been enabled for single sign-on to Azure AD via an [Active Directory Federation Services (AD FS)](active-directory-aadconnect-user-signin.md) deployment. Both options require that you follow the tutorial following to enable single sign-on between Azure AD and Google Apps.


### Configuring Google Apps for single sign-on
1. Open a new tab in your browser, and sign into the [Google Apps Admin Console](http://admin.google.com/) using your administrator account.

2. Click **Security**. If you don't see the link, it may be hidden under the **More Controls** menu at the bottom of the screen.
   
    ![Click Security.][10]

3. On the **Security** page, click **Set up single sign-on (SSO).**
   
    ![Click SSO.][11]

4. Perform the following configuration changes:
   
    ![Configure SSO][12]
   
a. Select **Setup SSO with third-party identity provider**. 

b. Enter the following value in the **Sign-in page URL** field in Google Apps: %metadata:SingleSignOnServiceUrl% 

c. Enter the following value in the **Sign-out page URL** field in Google Apps: %metadata:SingleSignOutServiceUrl% 

d. Enter the following value in the **Change password URL** field in Google Apps: https://account.activedirectory.windowsazure.com/changepassword.aspx

e. In Google Apps, for the **Verification certificate**, upload the certificate that you downloaded in the step above. 

f. Click **Save Changes**.

## Quick Reference

* **Azure AD Single Sign-On Service URL**: %metadata:singleSignOnServiceUrl%

* **Azure AD Sign Out URL**: %metadata:singleSignOutServiceUrl%

* **[Download Azure AD Signing Certificate](%metadata:CertificateDownloadRawUrl%)**

[10]: ./media/gapps-security.png
[11]: ./media/security-gapps.png
[12]: ./media/gapps-sso-config.png

## Additional Resources

* [How to integrate Google Apps with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-google-apps-tutorial)
* [How to configure user provisioning with Google Apps](https://docs.microsoft.com/azure/active-directory/active-directory-saas-google-apps-provisioning-tutorial)