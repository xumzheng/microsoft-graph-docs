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
source := graphmodels.NewParticipantInfo()
odataType := "#microsoft.graph.participantInfo"
source.SetOdataType(&odataType) 
identity := graphmodels.NewIdentitySet()
odataType := "#microsoft.graph.identitySet"
identity.SetOdataType(&odataType) 
application := graphmodels.NewIdentity()
odataType := "#microsoft.graph.identity"
application.SetOdataType(&odataType) 
displayName := "Calling Bot"
application.SetDisplayName(&displayName) 
id := "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
application.SetId(&id) 
identity.SetApplication(application)
source.SetIdentity(identity)
region := null
source.SetRegion(&region) 
languageId := null
source.SetLanguageId(&languageId) 
requestBody.SetSource(source)


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
mediaConfig := graphmodels.NewMediaConfig()
odataType := "#microsoft.graph.appHostedMediaConfig"
mediaConfig.SetOdataType(&odataType) 
additionalData := map[string]interface{}{
	"blob" : "<Media Session Configuration>", 
}
mediaConfig.SetAdditionalData(additionalData)
requestBody.SetMediaConfig(mediaConfig)

result, err := graphClient.Communications().Calls().Post(requestBody)


```