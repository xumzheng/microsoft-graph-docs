---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	"@odata.type" = "#microsoft.graph.security.retentionLabel"
	DisplayName = "String"
	BehaviorDuringRetentionPeriod = "String"
	ActionAfterRetentionPeriod = "String"
	RetentionTrigger = "String"
	RetentionDuration = @{
		"@odata.type" = "microsoft.graph.security.retentionDuration"
	}
	IsInUse = "Boolean"
	DescriptionForAdmins = "String"
	DescriptionForUsers = "String"
	CreatedBy = @{
		"@odata.type" = "microsoft.graph.identitySet"
	}
	LabelToBeApplied = "String"
	DefaultRecordBehavior = "String"
}

Update-MgBetaSecurityLabelRetentionLabel -RetentionLabelId $retentionLabelId -BodyParameter $params

```