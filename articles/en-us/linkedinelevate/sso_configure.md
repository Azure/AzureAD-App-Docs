## Prerequisites

To configure Azure AD integration with Linkedin Elevate, you need the following items:

- An Azure AD subscription
- A Linkedin Elevate single-sign on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can get a one-month trial [here](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Linkedin Elevate for single sign-on

1. In a different web browser window, sign-on to your LinkedIn Elevate tenant as an administrator.

2. In **Account Center**, click **Global Settings** under **Settings**. Also, select **Elevate - Elevate AAD Test** from the dropdown list.

	![Configure Single Sign-On](./media/tutorial_linkedin_admin_01.png)

3. Click **OR Click Here to load and copy individual fields from the form** and copy **Entity Id** and **Assertion Consumer Access (ACS) Url**

	![Configure Single Sign-On](./media/tutorial_linkedin_admin_03.png)

4. Go to **LinkedIn Admin Settings** section. Upload the XML file you downloaded from the Azure portal by clicking the Upload XML file option.

	![Configure Single Sign-On](./media/tutorial_linkedin_metadata_03.png)

5. Click **On** to enable SSO. SSO status changes from **Not Connected** to **Connected**

	![Configure Single Sign-On](./media/tutorial_linkedin_admin_05.png)


## Quick Reference

* **Azure AD Single Sign-On Service URL** : %metadata:singleSignOnServiceUrl%

* **Azure AD SAML Entity ID** : %metadata:IssuerUri%

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Linkedin Elevate with Azure Active Directory](active-directory-saas-linkedinelevate-tutorial.md)
* [How to configure user provisioning with Linkedin Elevate](active-directory-saas-linkedinelevate-user-provisioning-tutorial.md)
