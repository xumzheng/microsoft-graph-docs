---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewEducationClass()
odataType := "#microsoft.graph.educationClass"
requestBody.SetOdataType(&odataType) 
displayName := "String"
requestBody.SetDisplayName(&displayName) 
mailNickname := "String"
requestBody.SetMailNickname(&mailNickname) 
description := "String"
requestBody.SetDescription(&description) 
createdBy := graphmodels.NewIdentitySet()
odataType := "microsoft.graph.identitySet"
createdBy.SetOdataType(&odataType) 
requestBody.SetCreatedBy(createdBy)
classCode := "String"
requestBody.SetClassCode(&classCode) 
externalName := "String"
requestBody.SetExternalName(&externalName) 
externalId := "String"
requestBody.SetExternalId(&externalId) 
externalSource := graphmodels.STRING_EDUCATIONEXTERNALSOURCE 
requestBody.SetExternalSource(&externalSource) 
externalSourceDetail := "String"
requestBody.SetExternalSourceDetail(&externalSourceDetail) 
grade := "String"
requestBody.SetGrade(&grade) 
term := graphmodels.NewEducationTerm()
odataType := "microsoft.graph.educationTerm"
term.SetOdataType(&odataType) 
requestBody.SetTerm(term)

result, err := graphClient.Education().Classes().Post(requestBody)


```