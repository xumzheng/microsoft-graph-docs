---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

Get-MgIdentityGovernanceAppConsentRequest -AppConsentRequestId $appConsentRequestId -Filter "userConsentRequests/any(u:u/status eq 'InProgress')" 

```