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
additionalData := map[string]interface{}{
applicationInstance := graphmodels.New()
odataType := "#microsoft.graph.identity"
applicationInstance.SetOdataType(&odataType) 
displayName := "Calling Bot"
applicationInstance.SetDisplayName(&displayName) 
id := "3d913abb-aec0-4964-8fa6-3c6850c4f278"
applicationInstance.SetId(&id) 
	identity.SetApplicationInstance(applicationInstance)
}
identity.SetAdditionalData(additionalData)
source.SetIdentity(identity)
countryCode := null
source.SetCountryCode(&countryCode) 
endpointType := null
source.SetEndpointType(&endpointType) 
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
additionalData := map[string]interface{}{
phone := graphmodels.New()
odataType := "#microsoft.graph.identity"
phone.SetOdataType(&odataType) 
id := "+12345678901"
phone.SetId(&id) 
	identity.SetPhone(phone)
}
identity.SetAdditionalData(additionalData)
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
tenantId := "aa67bd4c-8475-432d-bd41-39f255720e0a"
requestBody.SetTenantId(&tenantId) 

result, err := graphClient.Communications().Calls().Post(requestBody)


```