## Prerequisites

To configure Azure AD integration with JIRA SAML SSO by Microsoft, you need the following items:

- An Azure AD subscription
- A JIRA SAML SSO by Microsoft single sign-on enabled subscription

> **Note:**
> To test the steps in this tutorial, we do not recommend using a production environment.

To test the steps in this tutorial, you should follow these recommendations:

- Do not use your production environment, unless it is necessary.
- If you don't have an Azure AD trial environment, you can [get a one-month trial](https://azure.microsoft.com/pricing/free-trial/).

### Configuring JIRA SAML SSO by Microsoft for single sign-on

1. In a different web browser window, log in to your JIRA instance as an administrator.

2. Hover on cog and click the **Add-ons**.

	![Configure Single Sign-On](.\media\addon1.png)

3. Download the plugin from [Microsoft Download Center](https://www.microsoft.com/en-us/download/details.aspx?id=56506). Manually upload the plugin provided by Microsoft using **Upload add-on** menu. The download of plugin is covered under [Microsoft Service Agreement](https://www.microsoft.com/en-us/servicesagreement/).

	![Configure Single Sign-On](.\media\addon12.png)

4. Once the plugin is installed, it appears in **User Installed** add-ons section of **Manage Add-on** section. Click **Configure** to configure the new plugin.

	![Configure Single Sign-On](.\media\addon13.png)

5. Perform following steps on configuration page:

	![Configure Single Sign-On](.\media\addon52.png)

	> [!TIP]
	> Ensure that there is only one certificate mapped against the app so that there is no error in resolving the metadata. If there are multiple certificates, upon resolving the metadata, admin gets an error.

	a. In the **Metadata URL** textbox, paste **[Downloaded SAML Metadata file](%metadata:metadataDownloadUrl%)** value which you have copied from the Azure portal and click the **Resolve** button. It reads the IdP metadata URL and populates all the fields information.

	b. Copy the **Identifier, Reply URL and Sign on URL** values and paste them in **Identifier, Reply URL and Sign on URL** textboxes respectively in **JIRA SAML SSO by Microsoft Domain and URLs** section on Azure portal.

	c. In **Login Button Name** type the name of button your organization wants the users to see on login screen.

	d. In **SAML User ID Locations** select either **User ID is in the NameIdentifier element of the Subject statement** or **User ID is in an Attribute element**.  This ID has to be the JIRA user id. If the user id is not matched, then system will not allow users to log in.

	> [!Note]
	> Default SAML User ID location is Name Identifier. You can change this to an attribute option and enter the appropriate attribute name.

	e. If you select **User ID is in an Attribute element** option, then in **Attribute name** textbox type the name of the attribute where User Id is expected.

	f. If you are using the federated domain (like ADFS etc.) with Azure AD, then click on the **Enable Home Realm Discovery** option and configure the **Domain Name**.

	g. In **Domain Name** type the domain name here in case of the ADFS-based login.

	h. Check **Enable Single Sign out** if you wish to log out from Azure AD when a user logs out from JIRA.

	i. Click **Save** button to save the settings.

	> [!NOTE]
	> For more information about installation and troubleshooting, visit [MS JIRA SSO Connector Admin Guide](ms-confluence-jira-plugin-adminguide.md) and there is also [FAQ](ms-confluence-jira-plugin-faq.md) for your assistance

## Quick Reference

* **[Download Azure AD Signing Certifcate](%metadata:CertificateDownloadRawUrl%)**

* **[Download SAML Metadata file](%metadata:metadataDownloadUrl%)**

## Additional Resources

* [How to integrate JIRA SAML SSO by Microsoft with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-jiramicrosoft-tutorial)
