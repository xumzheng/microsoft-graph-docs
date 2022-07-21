---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewConversationMember()
odataType := "#microsoft.graph.aadUserConversationMember"
requestBody.SetOdataType(&odataType) 
roles := []string {

}
requestBody.SetRoles(roles)
additionalData := map[string]interface{}{
	"odataBind" : "https://graph.microsoft.com/beta/users/24b3819b-4e1d-4f3e-86bd-e42b54d0b2b4", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.TeamsById("team-id").ChannelsById("channel-id").Members().Post(requestBody)


```