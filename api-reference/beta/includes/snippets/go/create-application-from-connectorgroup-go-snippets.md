---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceUpdate()
odataId := "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.ApplicationsById("application-id").ConnectorGroup().$ref().Put(requestBody)


```