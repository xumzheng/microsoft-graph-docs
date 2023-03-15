---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	Description = "Configure new hire tasks for onboarding employees on their first day"
	DisplayName = "Australia Onboard new hire employee"
	IsEnabled = $true
	IsSchedulingEnabled = $false
}

Update-MgBetaIdentityGovernanceLifecycleWorkflow -WorkflowId $workflowId -BodyParameter $params

```