<a href="https://github.com/byt3n33dl3/SharkMapExec/"><p align="center">
<img width="300" height="300" src="/inc/sahrk.png">
</p></a>

<div align="center">
<h2>BlackMarlinExec Attack Kit</h2>
<p></div>


<p align="center">
  <a href="https://github.com/Marten4n6/EvilOSX/blob/master/LICENSE.txt">
      <img src="https://img.shields.io/badge/license-BSD3-yellow.svg?style=flat-square" alt="License">
  </a>
  <a href="https://github.com/Marten4n6/EvilOSX/blob/master/LICENSE.txt">
      <img src="https://img.shields.io/badge/Offensive-red.svg?style=flat-square" alt="LPT-Master">
  </a>
  <a href="https://github.com/Marten4n6/EvilOSX/blob/master/LICENSE.txt">
      <img src="https://img.shields.io/badge/Powershell-blue.svg?style=flat-square" alt="Python">
  </a>
  <a href="https://github.com/Marten4n6/EvilOSX/issues">
    <img src="https://img.shields.io/github/issues/Marten4n6/EvilOSX.svg?style=flat-square" alt="Issues">
  </a>
  <a href="https://github.com/Marten4n6/EvilOSX/blob/master/CONTRIBUTING.md">
      <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square" alt="Contributing">
  </a>
</p>

This is a **BlackkMapExec** Attacks Kit.

You are on the **latest Up to Date** repository of the project SharkMapExec

- If you want to report a problem, open un [Issue](https://github.com/byt3n33dl3/SharkMapExec/issues) 
- If you want to contribute, open a [Pull Request](https://github.com/byt3n33dl3/SharkMapExec/pulls)
- If you want to discuss, open a [Discussion](https://github.com/byt3n33dl3/SharkMapExec/discussions)

Token Management and Manipulation Functions
-------------------------------------------
* ``Get-AzureKeyVaultTokenWithClientCredentials`` requests a token from STS with Azure Vault specified as the resource/intended audience using a client ID and secret.
* ``Get-AzureKeyVaultTokenWithUsernamePassword`` requests a token from STS with Azure Vault specified as the resource/intended audience using a user-supplied username and password.
* ``Get-AzurePortalTokenWithRefreshToken`` requests an Azure Portal Auth Refresh token with a user-supplied refresh token.
* ``Get-AzureRMTokenWithClientCredentials`` requests an AzureRM-scoped JWT with a client ID and secret. Useful for authenticating as an Entra service principal.
* ``Get-AzureRMTokenWithPortalAuthRefreshToken`` requests an AzureRM-scoped JWT with a user-supplied Azure Portal Auth Refresh token.
* ``Get-AzureRMTokenWithRefreshToken`` requests an AzureRM-scoped JWT with a user-supplied refresh token.
* ``Get-AzureRMTokenWithUsernamePassword`` requests an AzureRM-scoped JWT with a user-supplied username and password.
* ``Get-EntraRefreshTokenWithUsernamePassword`` requests a collection of tokens, including a refresh token, from login.microsoftonline.com with a user-supplied username and password. This will fail if the user has Multi-Factor Authentication requirements or is affected by a Conditional Access Policy.
* ``Get-MSGraphTokenWithClientCredentials`` requests an MS Graph-scoped JWT with a client ID and secret. Useful for authenticating as an Entra service principal.
* ``Get-MSGraphTokenWithPortalAuthRefreshToken`` requests an MS Graph-scoped JWT with a user-supplied Azure Portal Auth Refresh token.
* ``Get-MSGraphTokenWithRefreshToken`` requests an MS Graph-scoped JWT with a user-supplied refresh token.
* ``Get-MSGraphTokenWithUsernamePassword`` requests an MS Graph-scoped JWT with a user-supplied username and password.
* ``Parse-JWTToken`` will take a Base64 encoded JWT as input and parse it for you. Useful for verifying correct token audience and claims.

The refresh token-based functions in SharkMapExec are based on functions in [TokenTactics](https://github.com/rvrsh3ll/TokenTactics) by Steve [Borosh](https://twitter.com/424f424f).

Entra Enumeration Functions
---------------------------
* ``Get-AllEntraApps`` collects all Entra application registration objects.
* ``Get-AllEntraGroups`` collects all Entra groups.
* ``Get-AllEntraRoles`` collects all Entra admin roles.
* ``Get-AllEntraServicePrincipals`` collects all Entra service principal objects.
* ``Get-AllEntraUsers`` collects all Entra users.
* ``Get-EntraAppOwner`` collects owners of an Entra app registration.
* ``Get-EntraDeviceRegisteredUsers`` collects users of an Entra device.
* ``Get-EntraGroupMembers`` collects members of an Entra group.
* ``Get-EntraGroupOwner`` collects owners of an Entra group.
* ``Get-EntraRoleTemplates`` collects Entra admin role templates.
* ``Get-EntraServicePrincipal`` collects an Entra service principal.
* ``Get-EntraServicePrincipalOwner`` collects owners of an Entra service principal.
* ``Get-EntraTierZeroServicePrincipals`` collects Entra service principals that have a Tier Zero Entra Admin Role or Tier Zero MS Graph App Role assignment.
* ``Get-MGAppRoles`` collects the app roles made available by the MS Graph service principal.

Azure Resource Manager Enumeration Functions
--------------------------------------------
* ``Get-AllAzureManagedIdentityAssignments`` collects all managed identity assignments. 
* ``Get-AllAzureRMAKSClusters`` collects all kubernetes service clusters under a subscription.
* ``Get-AllAzureRMAutomationAccounts`` collects all automation accounts under a subscription.
* ``Get-AllAzureRMAzureContainerRegistries`` collects all container registies under a subscription.
* ``Get-AllAzureRMFunctionApps`` collects all function apps under a subscription.
* ``Get-AllAzureRMKeyVaults`` collects all key vaults under a subscription.
* ``Get-AllAzureRMLogicApps`` collects all logic apps under a subscription.
* ``Get-AllAzureRMResourceGroups`` collects all resouce groups under a subscription.
* ``Get-AllAzureRMSubscriptions`` collects all AzureRM subscriptions.
* ``Get-AllAzureRMVMScaleSetsVMs`` collects all virtual machines under a VM scale set.
* ``Get-AllAzureRMVMScaleSets`` collects all virtual machine scale sets under a subscription.
* ``Get-AllAzureRMVirtualMachines`` collects all virtual machines under a subscription.
* ``Get-AllAzureRMWebApps`` collects all web apps under a subscription.
* ``Get-AzureAutomationAccountRunBookOutput`` runs an automation account runbook and retrieves its output.
* ``Get-AzureFunctionAppFunctionFile`` collects the raw file (usually source code) of a function app function.
* ``Get-AzureFunctionAppFunctions`` collects all functions under a function app.
* ``Get-AzureFunctionAppMasterKeys`` collects all master keys under a function app.
* ``Get-AzureFunctionOutput`` runs a function app function and retrieves its output.
* ``Get-AzureRMKeyVaultSecretValue`` collects a key vault secret value.
* ``Get-AzureRMKeyVaultSecretVersions`` collects all versions of a key vault secret.
* ``Get-AzureRMKeyVaultSecrets`` collects all secrets under a key vault.
* ``Get-AzureRMRoleAssignments`` collects all role assignments against an object.
* ``Get-AzureRMRoleDefinitions`` collects all role definitions described at a subscription scope, including custom roles.
* ``Get-AzureRMWebApp`` collects a web app.

Intune Enumeration Functions
----------------------------
* ``Get-IntuneManagedDevices`` collects Intune-managed devices.
* ``Get-IntuneRoleDefinitions`` collects available Intune role definitions.

Entra Abuse Functions
---------------------
* ``Add-MemberToEntraGroup`` will attempt to add a principal to an Entra group.
* ``Enable-EntraRole`` will attempt to enables (or "activate") the Entra role.
* ``New-EntraAppOwner`` will attempt to add a new owner to an Entra app.
* ``New-EntraAppRoleAssignment`` will attempt to grant an app role to a service principal. For example, you can use this to grant a service principal the RoleManagement.ReadWrite.Directory app role.
* ``New-EntraAppSecret`` will attempt to create a new secret for an existing Entra app registration.
* ``New-EntraGroupOwner`` will attempt to add a new owner to an Entra group.
* ``New-EntraRoleAssignment`` will attempt to assign an Entra admin role to a specified principal.
* ``New-EntraServicePrincipalOwner`` will attempt to will attempt to add a new owner to an Entra service principal.
* ``New-EntraServicePrincipalSecret`` will attempt to create a new secret for an existing Entra service principal.
* ``Reset-EntraUserPassword`` will attempt to reset the password of another user. If successful, the output will contain the new, Azure-generated password of the user.
* ``Set-EntraUserPassword`` will attempt to set the password of another user to a new user-provided value.

Azure Resource Manager Abuse Functions
--------------------------------------
* ``Invoke-AzureRMAKSRunCommand`` will instruct the AKS cluster to execute a command.
* ``Invoke-AzureRMVMRunCommand`` will attempt to execute a command on a VM.
* ``Invoke-AzureRMWebAppShellCommand`` will attempt to execute a command on a web app container.
* ``Invoke-AzureVMScaleSetVMRunCommand`` will attempt to execute a command on a VM Scale Set VM.
* ``New-AzureAutomationAccountRunBook`` will attempt to add a runbook to an automation account.
* ``New-AzureKeyVaultAccessPolicy`` will attempt to grant a principal "Get" and "List" permissions on a key vault's secrets, keys, and certificates.
* ``New-AzureRMRoleAssignment`` will attempt to grant a user-specified AzureRM role assignment to a particular principal over a certain scope.
* ``New-PowerShellFunctionAppFunction`` will attempt to create a new PowerShell function in a function app.

Meta Functions
--------------
* ``ConvertTo-Markdown`` is used for massaging output from the Invoke-Tests functions for usage in another platform.
* ``Invoke-AllAzureMGAbuseTests`` performs all abuse validation tests that can be executed by holding an MS Graph app role. Returns an object describing which privileges were successful at performing each abuse test.
* ``Invoke-AllAzureRMAbuseTests`` performs all AzureRM abuse validation tests and outputs a resulting object that describes which AzureRM roles granted the ability to perform each abuse.
* ``Invoke-AllEntraAbuseTests`` performs all abuse validation tests that can be executed by principals granted Entra admin roles. Returns an object describing which privileges were successful at performing each abuse test.
* ``New-EntraIDAbuseTestSPs`` creates a new service principal per active Entra admin role and grants each service principal the appropriate role. Returns plain text credentials created for each service prinicpal.
* ``New-EntraIDAbuseTestUsers`` creates a new user per active Entra admin role and grants each user the appropriate role. Returns plain text credentials created for each user.
* ``New-IntuneAbuseTestUsers`` creates a new user per Intune role and grants each user the appropriate role. Returns plain text credentials created for each user.
* ``New-MSGraphAppRoleTestSPs`` creates a new service principal per MS Graph app role and grants each service principal the appropriate role. Returns plain text credentials created for each service prinicpal.
* ``New-TestAppReg`` creates an application registration object for the explicit purpose of abuse validation testing.
* ``New-TestSP`` creates a new service principal and associates it with the app created by the above function.
* ``Remove-AbuseTestAzureRMRoles`` is a clean-up function for removing AzureRM admin roles created during testing.
* ``Remove-AbuseTestServicePrincipals`` cleans up abuse tests by removing the serivce principals that were created during testing.
* ``Test-AzureRMAddSelfToAzureRMRole`` used in abuse validation testing to determine whether a service principal with certain rights can grant itself the User Access Admin role over a subscription.
* ``Test-AzureRMCreateFunction`` used in abuse validation testing to test if a service principal can add a new function to an existing function app.
* ``Test-AzureRMPublishAutomationAccountRunBook`` is used to test whether a service principal can publish a new runbook to an existing automation account.
* ``Test-AzureRMVMRunCommand`` is used to test whether a principal can run a command on an existing VM.
* ``Test-MGAddMemberToNonRoleEligibleGroup`` is used to test whether the service principal can add itself to a non-role eligible group.
* ``Test-MGAddMemberToRoleEligibleGroup`` is used to test whether the service principal can add itself to a role eligible group.
* ``Test-MGAddOwnerToNonRoleEligibleGroup`` is used to test whether a service principal can grant itself explicit ownership of a non-role eligible group.
* ``Test-MGAddOwnerToRoleEligibleGroup`` is used to test whether a service principal can grant itself explicit ownership of a role eligiblee group.
* ``Test-MGAddRootCACert`` is used to test whether a service principal can add a new Root CA cert to the tenant.
* ``Test-MGAddSecretToApp`` is used to test whether the service principal can add a new secret to an existing app.
* ``Test-MGAddSecretToSP`` is used to test whether the service principal can add a new secret to an existing service principal.
* ``Test-MGAddSelfAsOwnerOfApp`` is used in abuse validation testing to determine whether a service principal with a particular privilege can grant itself ownership of an existing Entra app.
* ``Test-MGAddSelfAsOwnerOfSP`` is used in abuse validation testing to determine whether a service principal with a particular privilege can grant itself ownership of an existing Entra service principal.
* ``Test-MGAddSelfToEntraRole`` is used in abuse validation testing to determine whether a service principal with a particular privilege can add itself to an Entra admin role - Global Admin, for example.
* ``Test-MGAddSelfToMGAppRole``is used in abuse validation testing to determine whether a service principal with a particular privilege can grant itself a particular MS Graph app role without admin consent.