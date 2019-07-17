## Prerequisites

To configure Azure AD integration with Abstract, you need the following items:

- An Azure AD subscription
- An Abstract single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a [free account](https://azure.microsoft.com/free/).

### Configuring Abstract for single sign-on

Make sure to retrieve your `App Federation Metadata Url` and the `Azure AD Identifier` from the Azure portal, as you will need those to configure SSO on Abstract.

You will find those information on the **Set up Single Sign-On with SAML** page:

* The `App Federation Metadata Url` is located in the **SAML Signing Certificate** section.
* The `Azure AD Identifier` is located in the **Set up Abstract** section.


You are now ready to configure SSO on Abstract:

>[!Note]
>You will need to authenticate with an organization Admin account to access the SSO settings on Abstract.

1. Open the [Abstract web app](https://app.abstract.com/).
2. Go to the **Permissions** page in the left side bar.
3. In the **Configure SSO** section, enter your **Metadata URL** and **Entity ID**.
4. Enter any manual exceptions you might have. Emails listed in the manual exceptions section will bypass SSO and be able to log in with email and password. 
5. Click **Save Changes**.

>[!Note] 
>You’ll need to use primary email addresses in the manual exceptions list. SSO activation will fail if the email you list is a user’s secondary email. If that happens, you’ll see an error message with the primary email for the failing account. Add that primary email to the manual exceptions list after you’ve verified you know the user.

## Quick Reference

* **Login URL** : %metadata:singleSignOnServiceUrl%

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Abstract with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/abstract-tutorial)
