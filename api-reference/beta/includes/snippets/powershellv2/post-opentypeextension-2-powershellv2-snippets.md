---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	"@odata.type" = "microsoft.graph.openTypeExtension"
	ExtensionName = "Com.Contoso.Referral"
	CompanyName = "Wingtip Toys"
	DealValue = 
	ExpirationDate = "2015-12-03T10:00:00.000Z"
}

# A UPN can also be used as -UserId.
New-MgBetaUserMessageExtension -UserId $userId -MessageId $messageId -BodyParameter $params

```