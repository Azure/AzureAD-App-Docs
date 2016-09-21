##Configure %metadata:DisplayName% for single sign on

For users to be able to sign in using their organization account, %metadata:DisplayName% must be manually configured to use your Azure Active Directory as a SAML identity provider. %metadata:DisplayName% cannot prompt or otherwise allow users to sign in using Azure Active Directory if it has not been configured to do so.

To configure %metadata:DisplayName% for single sign-on:

1. Review the process for configuring SAML identity providers in %metadata:DisplayName%. To determine the correct process, view the documentation for %metadata:DisplayName% or contact your %metadata:DisplayName% representative for more information.

2. **Note:** Some guidance on how to configure %metadata:DisplayName% can be found on Azure.com, and we are in the process of migrating the application-specific steps to this guide. The older article on how to configure %metadata:DisplayName% can be found here, where only the steps related to uploading the Azure AD files and URLs to %metadata:DisplayName% need to be followed.

3. During this process, you will be prompted to provide files and URLs that correspond to Azure Active Directory. When prompted, use the files and URLs shown below:

    - **SignInUrlExample: ** %metadata:SignInUrlExample%

    - **singleSignOnServiceUrl:** %metadata:singleSignOnServiceUrl%

    - **singleSignOutServiceUrl:** %metadata:singleSignOutServiceUrl%

    - **IssuerUri:** %metadata:IssuerUri%

    - **Key:** %metadata:Key%

    - [certificateDownloadBase64Url](%metadata:certificateDownloadBase64Url%)

    - [CertificateDownloadRawUrl](%metadata:CertificateDownloadRawUrl%)

    - [metadataDownloadUrl](%metadata:metadataDownloadUrl%)

4. Once this information has been provided and configured in %metadata:DisplayName%, %metadata:DisplayName% will begin to require or otherwise allow users to sign in using your instance of Azure Active Directory.

##Prerequisites

1. You must have a valid tenant or subscription with %metadata:DisplayName%

2. Your tenant or subscription must provide the ability to configure a third-party SAML identity provider. To determine this, view your application’s documentation or contact the application provider.

