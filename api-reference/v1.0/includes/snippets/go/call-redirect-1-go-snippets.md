---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewRedirectPostRequestBody()


invitationParticipantInfo := graphmodels.NewInvitationParticipantInfo()
additionalData := map[string]interface{}{
	"odataType" : "#microsoft.graph.invitationParticipantInfo", 
identity := graphmodels.New()
odataType := "#microsoft.graph.identitySet"
identity.SetOdataType(&odataType) 
application := graphmodels.New()
odataType := "#microsoft.graph.identity"
application.SetOdataType(&odataType) 
displayName := "test bot 2"
application.SetDisplayName(&displayName) 
id := "22bfd41f-550e-477d-8789-f6f7bd2a5e8b"
application.SetId(&id) 
	identity.SetApplication(application)
	invitationParticipantInfo.SetIdentity(identity)
}
invitationParticipantInfo.SetAdditionalData(additionalData)

targets := []graphmodels.InvitationParticipantInfoable {
	invitationParticipantInfo,

}
requestBody.SetTargets(targets)
callbackUri := "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
requestBody.SetCallbackUri(&callbackUri) 

graphClient.Communications().CallsById("call-id").Redirect().Post(requestBody)


```