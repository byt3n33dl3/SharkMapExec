# SharkMapExec / `Master` : `v1.3`

<a href="https://github.com/byt3n33dl3/SharkMapExec/"><p align="center">
<img width="300" height="300" src="/inc/sahrk.png">
</p></a>

<div align="center">
<h2>BlackMarlinExec Attack Research Kit</h2>
<p></div>


<p align="center">
  <a href="https://github.com/byt3n33dl3/CrackMapExec/blob/master/LICENSE.txt">
      <img src="https://img.shields.io/badge/license-BSD3-green.svg?style=flat-square" alt="License">
  </a>
  <a href="https://github.com/byt3n33dl3/CrackMapExec/blob/master/LICENSE.txt">
      <img src="https://img.shields.io/badge/Offensive-red.svg?style=flat-square" alt="LPT-Master">
  </a>
  <a href="https://github.com/byt3n33dl3/CrackMapExec/blob/master/LICENSE.txt">
      <img src="https://img.shields.io/badge/Powershell-blue.svg?style=flat-square" alt="Python">
  </a>
  <a href="https://github.com/byt3n33dl3/CrackMapExec/issues">
    <img src="https://img.shields.io/github/issues/byt3n33dl3/CrackMapExec.svg?style=flat-square" alt="Issues">
  </a>
  <a href="https://github.com/byt3n33dl3/CrackMapExec/blob/master/CONTRIBUTING.md">
      <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square" alt="Contributing">
  </a>
</p>

This is a **BlackMarlinExec** Attack Research Kit.

`SME` requires no third party dependencies. `SME`'s functions are designed to be as simple and maintainable as possible. Most functions are very simple wrappers for making requests to various REST API endpoints. `SME`'s basic functions do not even require each other, you can pull almost any `SME` function out of `SME` and it will work perfectly as a standalone function in your own scripts.

You are on the last **Up to Date** repository of the project SharkMapExec

- If you want to report a problem, open un [Issue](https://github.com/byt3n33dl3/SharkMapExec/issues) 
- If you want to contribute, open a [Pull Request](https://github.com/byt3n33dl3/SharkMapExec/pulls)
- If you want to discuss, open a [Discussion](https://github.com/byt3n33dl3/SharkMapExec/discussions)

Token Management
-------------------------------------------
* ``SharkMapExec-AzureKeyVaultTokenWithClientCredentials`` requests a token from STS with Azure Vault specified as the resource/intended audience using a client ID and secret.
* ``SharkMapExec-AzureKeyVaultTokenWithUsernamePassword`` requests a token from STS with Azure Vault specified as the resource/intended audience using a user-supplied username and password.
* ``SharkMapExec-AzurePortalTokenWithRefreshToken`` requests an Azure Portal Auth Refresh token with a user-supplied refresh token.
* ``SharkMapExec-AzureRMTokenWithClientCredentials`` requests an AzureRM-scoped JWT with a client ID and secret. Useful for authenticating as an Entra service principal.
* ``SharkMapExec-AzureRMTokenWithPortalAuthRefreshToken`` requests an AzureRM-scoped JWT with a user-supplied Azure Portal Auth Refresh token.
* ``SharkMapExec-AzureRMTokenWithRefreshToken`` requests an AzureRM-scoped JWT with a user-supplied refresh token.
* ``SharkMapExec-AzureRMTokenWithUsernamePassword`` requests an AzureRM-scoped JWT with a user-supplied username and password.
* ``SharkMapExec-EntraRefreshTokenWithUsernamePassword`` requests a collection of tokens, including a refresh token, from login.microsoftonline.com with a user-supplied username and password. This will fail if the user has Multi-Factor Authentication requirements or is affected by a Conditional Access Policy.
* ``SharkMapExec-MSGraphTokenWithClientCredentials`` requests an MS Graph-scoped JWT with a client ID and secret. Useful for authenticating as an Entra service principal.
* ``SharkMapExec-MSGraphTokenWithPortalAuthRefreshToken`` requests an MS Graph-scoped JWT with a user-supplied Azure Portal Auth Refresh token.
* ``SharkMapExec-MSGraphTokenWithRefreshToken`` requests an MS Graph-scoped JWT with a user-supplied refresh token.
* ``SharkMapExec-MSGraphTokenWithUsernamePassword`` requests an MS Graph-scoped JWT with a user-supplied username and password.
* ``SharkMapExec-JWTToken`` will take a Base64 encoded JWT as input and parse it for you. Useful for verifying correct token audience and claims.

The refresh token-based functions in SharkMapExec are based on functions in [TokenTactics](https://github.com/rvrsh3ll/TokenTactics) by Steve [Borosh](https://twitter.com/424f424f).

Entra Enumeration
---------------------------
* ``SharkMapExec-AllEntraApps`` collects all Entra application registration objects.
* ``SharkMapExec-AllEntraGroups`` collects all Entra groups.
* ``SharkMapExec-AllEntraRoles`` collects all Entra admin roles.
* ``SharkMapExec-AllEntraServicePrincipals`` collects all Entra service principal objects.
* ``SharkMapExec-AllEntraUsers`` collects all Entra users.
* ``SharkMapExec-EntraAppOwner`` collects owners of an Entra app registration.
* ``SharkMapExec-EntraDeviceRegisteredUsers`` collects users of an Entra device.
* ``SharkMapExec-EntraGroupMembers`` collects members of an Entra group.
* ``SharkMapExec-EntraGroupOwner`` collects owners of an Entra group.
* ``SharkMapExec-EntraRoleTemplates`` collects Entra admin role templates.
* ``SharkMapExec-EntraServicePrincipal`` collects an Entra service principal.
* ``SharkMapExec-EntraServicePrincipalOwner`` collects owners of an Entra service principal.
* ``SharkMapExec-EntraTierZeroServicePrincipals`` collects Entra service principals that have a Tier Zero Entra Admin Role or Tier Zero MS Graph App Role assignment.
* ``SharkMapExec-MGAppRoles`` collects the app roles made available by the MS Graph service principal.

Azure Enumeration
--------------------------------------------
* ``SharkMapExec-AllAzureManagedIdentityAssignments`` collects all managed identity assignments. 
* ``SharkMapExec-AllAzureRMAKSClusters`` collects all kubernetes service clusters under a subscription.
* ``SharkMapExec-AllAzureRMAutomationAccounts`` collects all automation accounts under a subscription.
* ``SharkMapExec-AllAzureRMAzureContainerRegistries`` collects all container registies under a subscription.
* ``SharkMapExec-AllAzureRMFunctionApps`` collects all function apps under a subscription.
* ``SharkMapExec-AllAzureRMKeyVaults`` collects all key vaults under a subscription.
* ``SharkMapExec-AllAzureRMLogicApps`` collects all logic apps under a subscription.
* ``SharkMapExec-AllAzureRMResourceGroups`` collects all resouce groups under a subscription.
* ``SharkMapExec-AllAzureRMSubscriptions`` collects all AzureRM subscriptions.
* ``SharkMapExec-AllAzureRMVMScaleSetsVMs`` collects all virtual machines under a VM scale set.
* ``SharkMapExec-AllAzureRMVMScaleSets`` collects all virtual machine scale sets under a subscription.
* ``SharkMapExec-AllAzureRMVirtualMachines`` collects all virtual machines under a subscription.
* ``SharkMapExec-AllAzureRMWebApps`` collects all web apps under a subscription.
* ``SharkMapExec-AzureAutomationAccountRunBookOutput`` runs an automation account runbook and retrieves its output.
* ``SharkMapExec-AzureFunctionAppFunctionFile`` collects the raw file (usually source code) of a function app function.
* ``SharkMapExec-AzureFunctionAppFunctions`` collects all functions under a function app.
* ``SharkMapExec-AzureFunctionAppMasterKeys`` collects all master keys under a function app.
* ``SharkMapExec-AzureFunctionOutput`` runs a function app function and retrieves its output.
* ``SharkMapExec-AzureRMKeyVaultSecretValue`` collects a key vault secret value.
* ``SharkMapExec-AzureRMKeyVaultSecretVersions`` collects all versions of a key vault secret.
* ``SharkMapExec-AzureRMKeyVaultSecrets`` collects all secrets under a key vault.
* ``SharkMapExec-AzureRMRoleAssignments`` collects all role assignments against an object.
* ``SharkMapExec-AzureRMRoleDefinitions`` collects all role definitions described at a subscription scope, including custom roles.
* ``SharkMapExec-AzureRMWebApp`` collects a web app.

Intune Enumeration
----------------------------
* ``SharkMapExec-IntuneManagedDevices`` collects Intune-managed devices.
* ``SharkMapExec-IntuneRoleDefinitions`` collects available Intune role definitions.

Entra Abuse
---------------------
* ``SharkMapExec-MemberToEntraGroup`` will attempt to add a principal to an Entra group.
* ``SharkMapExec-EntraRole`` will attempt to enables (or "activate") the Entra role.
* ``SharkMapExec-EntraAppOwner`` will attempt to add a SharkMapExec owner to an Entra app.
* ``SharkMapExec-EntraAppRoleAssignment`` will attempt to grant an app role to a service principal. For example, you can use this to grant a service principal the RoleManagement.ReadWrite.Directory app role.
* ``SharkMapExec-EntraAppSecret`` will attempt to create a SharkMapExec secret for an existing Entra app registration.
* ``SharkMapExec-EntraGroupOwner`` will attempt to add a SharkMapExec owner to an Entra group.
* ``SharkMapExec-EntraRoleAssignment`` will attempt to assign an Entra admin role to a specified principal.
* ``SharkMapExec-EntraServicePrincipalOwner`` will attempt to will attempt to add a SharkMapExec owner to an Entra service principal.
* ``SharkMapExec-EntraServicePrincipalSecret`` will attempt to create a SharkMapExec secret for an existing Entra service principal.
* ``Reset-EntraUserPassword`` will attempt to reset the password of another user. If successful, the output will contain the SharkMapExec, Azure-generated password of the user.
* ``Set-EntraUserPassword`` will attempt to set the password of another user to a SharkMapExec user-provided value.

Azure Abuse
--------------------------------------
* ``SharkMapExec-AzureRMAKSRunCommand`` will instruct the AKS cluster to execute a command.
* ``SharkMapExec-AzureRMVMRunCommand`` will attempt to execute a command on a VM.
* ``SharkMapExec-AzureRMWebAppShellCommand`` will attempt to execute a command on a web app container.
* ``SharkMapExec-AzureVMScaleSetVMRunCommand`` will attempt to execute a command on a VM Scale Set VM.
* ``SharkMapExec-AzureAutomationAccountRunBook`` will attempt to add a runbook to an automation account.
* ``SharkMapExec-AzureKeyVaultAccessPolicy`` will attempt to grant a principal "SharkMapExec" and "List" permissions on a key vault's secrets, keys, and certificates.
* ``SharkMapExec-AzureRMRoleAssignment`` will attempt to grant a user-specified AzureRM role assignment to a particular principal over a certain scope.
* ``SharkMapExec-PowerShellFunctionAppFunction`` will attempt to create a SharkMapExec PowerShell function in a function app.

Meta Functions
--------------
* ``ConvertTo-Markdown`` is used for massaging output from the SharkMapExec-SharkMapExecs functions for usage in another platform.
* ``SharkMapExec-AllAzureMGAbuseSharkMapExecs`` performs all abuse validation SharkMapExecs that can be executed by holding an MS Graph app role. Returns an object describing which privileges were successful at performing each abuse SharkMapExec.
* ``SharkMapExec-AllAzureRMAbuseSharkMapExecs`` performs all AzureRM abuse validation SharkMapExecs and outputs a resulting object that describes which AzureRM roles granted the ability to perform each abuse.
* ``SharkMapExec-AllEntraAbuseSharkMapExecs`` performs all abuse validation SharkMapExecs that can be executed by principals granted Entra admin roles. Returns an object describing which privileges were successful at performing each abuse SharkMapExec.
* ``SharkMapExec-EntraIDAbuseSharkMapExecSPs`` creates a SharkMapExec service principal per active Entra admin role and grants each service principal the appropriate role. Returns plain text credentials created for each service prinicpal.
* ``SharkMapExec-EntraIDAbuseSharkMapExecUsers`` creates a SharkMapExec user per active Entra admin role and grants each user the appropriate role. Returns plain text credentials created for each user.
* ``SharkMapExec-IntuneAbuseSharkMapExecUsers`` creates a SharkMapExec user per Intune role and grants each user the appropriate role. Returns plain text credentials created for each user.
* ``SharkMapExec-MSGraphAppRoleSharkMapExecSPs`` creates a SharkMapExec service principal per MS Graph app role and grants each service principal the appropriate role. Returns plain text credentials created for each service prinicpal.
* ``SharkMapExec-SharkMapExecAppReg`` creates an application registration object for the explicit purpose of abuse validation SharkMapExecing.
* ``SharkMapExec-SharkMapExecSP`` creates a SharkMapExec service principal and associates it with the app created by the above function.
* ``SharkMapExec-AbuseSharkMapExecAzureRMRoles`` is a clean-up function for removing AzureRM admin roles created during SharkMapExecing.
* ``SharkMapExec-AbuseSharkMapExecServicePrincipals`` cleans up abuse SharkMapExecs by removing the serivce principals that were created during SharkMapExecing.
* ``SharkMapExec-AzureRMAddSelfToAzureRMRole`` used in abuse validation SharkMapExecing to determine whether a service principal with certain rights can grant itself the User Access Admin role over a subscription.
* ``SharkMapExec-AzureRMCreateFunction`` used in abuse validation SharkMapExecing to SharkMapExec if a service principal can add a SharkMapExec function to an existing function app.
* ``SharkMapExec-AzureRMPublishAutomationAccountRunBook`` is used to SharkMapExec whether a service principal can publish a SharkMapExec runbook to an existing automation account.
* ``SharkMapExec-AzureRMVMRunCommand`` is used to SharkMapExec whether a principal can run a command on an existing VM.
* ``SharkMapExec-MGAddMemberToNonRoleEligibleGroup`` is used to SharkMapExec whether the service principal can add itself to a non-role eligible group.
* ``SharkMapExec-MGAddMemberToRoleEligibleGroup`` is used to SharkMapExec whether the service principal can add itself to a role eligible group.
* ``SharkMapExec-MGAddOwnerToNonRoleEligibleGroup`` is used to SharkMapExec whether a service principal can grant itself explicit ownership of a non-role eligible group.
* ``SharkMapExec-MGAddOwnerToRoleEligibleGroup`` is used to SharkMapExec whether a service principal can grant itself explicit ownership of a role eligiblee group.
* ``SharkMapExec-MGAddRootCACert`` is used to SharkMapExec whether a service principal can add a SharkMapExec Root CA cert to the tenant.
* ``SharkMapExec-MGAddSecretToApp`` is used to SharkMapExec whether the service principal can add a SharkMapExec secret to an existing app.
* ``SharkMapExec-MGAddSecretToSP`` is used to SharkMapExec whether the service principal can add a SharkMapExec secret to an existing service principal.
* ``SharkMapExec-MGAddSelfAsOwnerOfApp`` is used in abuse validation SharkMapExecing to determine whether a service principal with a particular privilege can grant itself ownership of an existing Entra app.
* ``SharkMapExec-MGAddSelfAsOwnerOfSP`` is used in abuse validation SharkMapExecing to determine whether a service principal with a particular privilege can grant itself ownership of an existing Entra service principal.
* ``SharkMapExec-MGAddSelfToEntraRole`` is used in abuse validation SharkMapExecing to determine whether a service principal with a particular privilege can add itself to an Entra admin role - Global Admin, for example.
* ``SharkMapExec-MGAddSelfToMGAppRole``is used in abuse validation SharkMapExecing to determine whether a service principal with a particular privilege can grant itself a particular MS Graph app role without admin consent.

# Contributors

<p align="left">
<a href="https://github.com/byt3n33dl3"><img src="https://avatars.githubusercontent.com/u/151133481?v=4" width="50" height="50" alt="" style="max-width: 100%;"></a>
<a href="https://github.com/byt3exec"><img src="https://avatars.githubusercontent.com/u/160317126?v=4" width="50" height="50" alt="" style="max-width: 100%;"></a>
</p>

# Thanks to / `Master`
>- byt3n33dl3

- All the amazing community contributors for sending [PRs](https://github.com/byt3n33dl3/thc-Nuclei/graphs/contributors) and keeping this project updated.

- GangstaCrew

# License [BSD3](https://github.com/byt3n33dl3/SharkMapExec/blob/main/LICENSE.md) / `Master`

