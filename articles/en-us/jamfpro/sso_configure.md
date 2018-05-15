## Prerequisites

To configure Azure AD integration with Jamf Pro SAML Connector, you need the following items:

- An Azure AD subscription
- A Jamf Pro SAML Connector single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring Jamf Pro SAML Connector for single sign-on

1. In a different web browser window, log into your Jamf Pro company site as an administrator.

2. Click on the **Settings icon** from the top right corner of the page.

	![Jamf Pro Configuration](./media/configure1.png)

3. Click on **Single Sign On**.

	![Jamf Pro Configuration](./media/configure2.png)

4. Scroll down upto **IDENTITY PROVIDER** under the **Single Sign-On** section and perform the following steps:

	![Jamf Pro Configuration](./media/configure3.png)

	a. Select **Other** as a option from the **IDENTITY PROVIDER** dropdown.

	b. In the **OTHER PROVIDER** textbox, enter **Azure AD**.

	c. Select **Metadata URL** as a option from the **IDENTITY PROVIDER METADATA SOURCE** dropdown and in the following textbox, paste the **App Federation Metadata Url** value which you have copied from the Azure portal.

	d. Copy the **Entity ID** vlaue and paste it into the **Identifier (Entity ID)** textbox in **Jamf Pro Domain and URLs** section on Azure portal.

	> **Note:**
	> Here `aadsso` is the subdomain part (which is for reference purpose). Use this value to complete the Sign-on URL and Reply URL in the **Jamf Pro Domain and URLs** section on Azure portal.

	e. Click **Save**.

## Quick Reference

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate Jamf Pro SAML Connector with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-jamfprosamlconnector-tutorial)
