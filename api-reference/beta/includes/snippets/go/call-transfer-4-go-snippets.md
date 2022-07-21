---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewTransferPostRequestBody()
transferTarget := graphmodels.NewInvitationParticipantInfo()
odataType := "#microsoft.graph.invitationParticipantInfo"
transferTarget.SetOdataType(&odataType) 
endpointType := graphmodels.DEFAULT_ENDPOINTTYPE 
transferTarget.SetEndpointType(&endpointType) 
identity := graphmodels.NewIdentitySet()
odataType := "#microsoft.graph.identitySet"
identity.SetOdataType(&odataType) 
additionalData := map[string]interface{}{
phone := graphmodels.New()
odataType := "#microsoft.graph.identity"
phone.SetOdataType(&odataType) 
id := "+12345678901"
phone.SetId(&id) 
	identity.SetPhone(phone)
}
identity.SetAdditionalData(additionalData)
transferTarget.SetIdentity(identity)
replacesCallId := "e5d39592-99bd-4db8-bca8-30fb894ec51d"
transferTarget.SetReplacesCallId(&replacesCallId) 
additionalData := map[string]interface{}{
	"languageId" : "en-us", 
	"region" : "amer", 
}
transferTarget.SetAdditionalData(additionalData)
requestBody.SetTransferTarget(transferTarget)

graphClient.Communications().CallsById("call-id").Transfer().Post(requestBody)


```