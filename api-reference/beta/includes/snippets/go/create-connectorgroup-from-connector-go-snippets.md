---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.OnPremisesPublishingProfilesById("onPremisesPublishingProfile-id").ConnectorsById("connector-id").MemberOf().$ref().Post(requestBody)


```