---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	"@odata.type" = "#microsoft.outlookServices.openTypeExtension"
	ExtensionName = "Com.Contoso.Estimate"
	CompanyName = "Contoso"
	ExpirationDate = "2016-07-30T11:00:00.000Z"
	DealValue = 
	TopPicks = @(
		"Employees only"
		"Add spouse or guest"
		"Add family"
	)
}

Update-MgBetaGroupThreadPostExtension -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -ExtensionId $extensionId -BodyParameter $params

```