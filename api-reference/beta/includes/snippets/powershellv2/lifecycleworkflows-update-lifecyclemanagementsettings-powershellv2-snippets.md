---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	"@odata.context" = "https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity"
	WorkflowScheduleIntervalInHours = 3
}

Update-MgBetaIdentityGovernanceLifecycleWorkflowSetting -BodyParameter $params

```