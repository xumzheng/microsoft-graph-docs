---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewCall()
odataType := "#microsoft.graph.call"
requestBody.SetOdataType(&odataType) 
direction := graphmodels.OUTGOING_CALLDIRECTION 
requestBody.SetDirection(&direction) 
callbackUri := "https://bot.contoso.com/callback"
requestBody.SetCallbackUri(&callbackUri) 
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
chatInfo := graphmodels.NewChatInfo()
odataType := "#microsoft.graph.chatInfo"
chatInfo.SetOdataType(&odataType) 
threadId := "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2"
chatInfo.SetThreadId(&threadId) 
messageId := "0"
chatInfo.SetMessageId(&messageId) 
requestBody.SetChatInfo(chatInfo)
meetingInfo := graphmodels.NewMeetingInfo()
odataType := "#microsoft.graph.organizerMeetingInfo"
meetingInfo.SetOdataType(&odataType) 
allowConversationWithoutHost := true
meetingInfo.SetAllowConversationWithoutHost(&allowConversationWithoutHost) 
additionalData := map[string]interface{}{
organizer := graphmodels.New()
odataType := "#microsoft.graph.identitySet"
organizer.SetOdataType(&odataType) 
user := graphmodels.New()
odataType := "#microsoft.graph.identity"
user.SetOdataType(&odataType) 
id := "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
user.SetId(&id) 
tenantId := "aa67bd4c-8475-432d-bd41-39f255720e0a"
user.SetTenantId(&tenantId) 
displayName := "Bob"
user.SetDisplayName(&displayName) 
	organizer.SetUser(user)
	meetingInfo.SetOrganizer(organizer)
}
meetingInfo.SetAdditionalData(additionalData)
requestBody.SetMeetingInfo(meetingInfo)
tenantId := "aa67bd4c-8475-432d-bd41-39f255720e0a"
requestBody.SetTenantId(&tenantId) 

result, err := graphClient.Communications().Calls().Post(requestBody)


```