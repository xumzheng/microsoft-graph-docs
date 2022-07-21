---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewCall()
odataType := "#microsoft.graph.call"
requestBody.SetOdataType(&odataType) 
callbackUri := "https://bot.contoso.com/callback"
requestBody.SetCallbackUri(&callbackUri) 


invitationParticipantInfo := graphmodels.NewInvitationParticipantInfo()
odataType := "#microsoft.graph.invitationParticipantInfo"
invitationParticipantInfo.SetOdataType(&odataType) 
identity := graphmodels.NewIdentitySet()
odataType := "#microsoft.graph.identitySet"
identity.SetOdataType(&odataType) 
user := graphmodels.NewIdentity()
odataType := "#microsoft.graph.identity"
user.SetOdataType(&odataType) 
displayName := "John"
user.SetDisplayName(&displayName) 
id := "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
user.SetId(&id) 
identity.SetUser(user)
invitationParticipantInfo.SetIdentity(identity)

targets := []graphmodels.InvitationParticipantInfoable {
	invitationParticipantInfo,

}
requestBody.SetTargets(targets)
requestedModalities := []graphmodels.Modalityable {
	"audio",

}
requestBody.SetRequestedModalities(requestedModalities)
callOptions := graphmodels.NewCallOptions()
odataType := "#microsoft.graph.outgoingCallOptions"
callOptions.SetOdataType(&odataType) 
isContentSharingNotificationEnabled := true
callOptions.SetIsContentSharingNotificationEnabled(&isContentSharingNotificationEnabled) 
requestBody.SetCallOptions(callOptions)
mediaConfig := graphmodels.NewMediaConfig()
odataType := "#microsoft.graph.serviceHostedMediaConfig"
mediaConfig.SetOdataType(&odataType) 
requestBody.SetMediaConfig(mediaConfig)

result, err := graphClient.Communications().Calls().Post(requestBody)


```