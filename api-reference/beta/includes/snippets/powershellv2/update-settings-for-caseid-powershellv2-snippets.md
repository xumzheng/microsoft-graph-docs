---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	RedundancyDetection = @{
		IsEnabled = $false
		SimilarityThreshold = 70
		MinWords = 12
		MaxWords = 400000
	}
	TopicModeling = @{
		IsEnabled = $false
		IgnoreNumbers = $false
		TopicCount = 50
		DynamicallyAdjustTopicCount = $false
	}
	Ocr = @{
		IsEnabled = $true
		MaxImageSize = 12000
	}
}

Update-MgBetaComplianceEdiscoveryCaseSetting -CaseId $caseId -BodyParameter $params

```