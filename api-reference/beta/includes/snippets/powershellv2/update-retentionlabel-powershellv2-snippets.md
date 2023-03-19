---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	"@odata.type" = "#microsoft.graph.security.retentionLabel"
	RetentionDuration = @{
		"@odata.type" = "microsoft.graph.security.retentionDuration"
	}
	DescriptionForAdmins = "String"
	DescriptionForUsers = "String"
	LabelToBeApplied = "String"
	DefaultRecordBehavior = "String"
}

Update-MgBetaSecurityLabelRetentionLabel -RetentionLabelId $retentionLabelId -BodyParameter $params

```