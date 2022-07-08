---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewContact()


typedEmailAddress := graphmodels.NewTypedEmailAddress()
additionalData := map[string]interface{}{
	"type" : "personal", 
	"name" : "Pavel Bansky", 
	"address" : "pavelb@adatum.onmicrosoft.com", 
}
typedEmailAddress.SetAdditionalData(additionalData)
typedEmailAddress1 := graphmodels.NewTypedEmailAddress()
additionalData := map[string]interface{}{
	"address" : "pavelb@fabrikam.onmicrosoft.com", 
	"name" : "Pavel Bansky", 
	"type" : "other", 
	"otherLabel" : "Volunteer work", 
}
typedEmailAddress1.SetAdditionalData(additionalData)

emailAddresses := []graphmodels.TypedEmailAddressable {
	typedEmailAddress,
	typedEmailAddress1,

}
requestBody.SetEmailAddresses(emailAddresses)

graphClient.Me().ContactsById("contact-id").Patch(requestBody)


```