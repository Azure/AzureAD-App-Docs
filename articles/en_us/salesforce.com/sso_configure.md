##Configure Salesforce for single sign on

1. To configure Azure Active Directory as an identity provider, log in to your Salesforce tenant above using your Salesforce administrator account.

2. Under the **Administrator** navigation pane, click **Security Controls** to expand the related section. Then click on **Single Sign-On Settings**.

	![Click on Single Sign-On Settings under Security Controls][10]

3. On the **Single Sign-On Settings** page, click the **Edit** button.

	![Click the Edit button][11]

	> [AZURE.NOTE] If you are unable to enable Single Sign-On settings for your Salesforce account, you may need to contact Salesforce's support in order to have the feature enabled for you.

4. Select **SAML Enabled**, and then click **Save**.

	![Select SAML Enabled][12]

5. To configure your SAML single sign-on settings, click **New**.

	![Select SAML Enabled][13]

6. On the **SAML Single Sign-On Setting Edit** page, enter the following values:

	![Screenshot of the configurations that you should make][14]

	- For the **Name** field, type in a friendly name for this configuration. Providing a value for **Name** automatically populate the **API Name** textbox.

	- For **Issuer**, enter the following value: %metadata:IssuerUri%

	- In the **Entity Id textbox**, type your Salesforce domain name using the following pattern:

	- Enterprise account: `https://<domain>.my.salesforce.com`

	- Developer account: `https://<domain>-dev-ed.my.salesforce.com`

	- Download the SAML certificate here: [Certificate download](%metadata:CertificateDownloadUrl%)

	- Then click **Browse** or **Choose File** to open the **Choose File to Upload** dialog, select the SAML certificate, and then click **Open** to upload the certificate.

	- For **SAML Identity Type**, select **Assertion contains User's salesforce.com username**.

	- For **SAML Identity Location**, select **Identity is in the NameIdentifier element of the Subject statement**

	- For **Identity Provider Login URL**, enter the following value: %metadata:SingleSignOnServiceUrl%

	- For **Service Provider Initiated Request Binding**, select **HTTP Redirect**.


	- Finally, click **Save** to apply your SAML single sign-on settings.

7. On the left navigation pane in Salesforce, click **Domain Management** to expand the related section, and then click **My Domain**.
	
	![Click on My Domain][15]

8. Scroll down to the **Authentication Configuration** section, and click the **Edit** button.

	![Click the Edit button][16]

9. In the **Authentication Service** section, select the friendly name of your SAML SSO configuration, and then click **Save**.

	![Select your SSO configuration][17]

	> [AZURE.NOTE] If more than one authentication service is selected, then when users attempt to initiate single sign-on to your Salesforce environment, they will be prompted to select which authentication service they would like to sign in with. If you don’t want this to happen, then you should **leave all other authentication services unchecked**.

[10]: media/sf-admin-sso.png
[11]: media/sf-admin-sso-edit.png
[12]: media/sf-enable-saml.png
[13]: media/sf-admin-sso-new.png
[14]: media/sf-saml-config.png
[15]: media/sf-my-domain.png
[16]: media/sf-edit-auth-config.png
[17]: media/sf-auth-config.png

##Prerequisites

You must have a valid tenant in [Salesforce.com](https://www.salesforce.com/). If you are using a Salesforce Sandbox environment, please see the [Salesforce Sandbox integration tutorial](https://go.microsoft.com/fwLink/?LinkID=521879).

Before you can configure single sign-on, you must set up and deploy a custom domain for your Salesforce environment. For instructions on how to do that, see [Set Up a Domain Name](https://help.salesforce.com/HTViewHelpDoc?id=domain_name_setup.htm&language=en_US).

> [IMPORTANT] If you are using a Salesforce.com **trial** account, then you will be unable to configure automated user provisioning. Trial accounts do not have the necessary API access enabled until they are purchased.

> You can get around this limitation by using a [free developer account](https://developer.salesforce.com/signup) to complete this tutorial.
