---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewEdiscoveryCaseSettings()
odataType := "#microsoft.graph.security.ediscoveryCaseSettings"
requestBody.SetOdataType(&odataType) 
redundancyDetection := graphmodels.NewRedundancyDetectionSettings()
odataType := "microsoft.graph.security.redundancyDetectionSettings"
redundancyDetection.SetOdataType(&odataType) 
requestBody.SetRedundancyDetection(redundancyDetection)
topicModeling := graphmodels.NewTopicModelingSettings()
odataType := "microsoft.graph.security.topicModelingSettings"
topicModeling.SetOdataType(&odataType) 
requestBody.SetTopicModeling(topicModeling)
ocr := graphmodels.NewOcrSettings()
odataType := "microsoft.graph.security.ocrSettings"
ocr.SetOdataType(&odataType) 
requestBody.SetOcr(ocr)

graphClient.Security().Cases().EdiscoveryCasesById("ediscoveryCase-id").Settings().Patch(requestBody)


```