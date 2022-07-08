---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewContact()
givenName := "Pavel"
requestBody.SetGivenName(&givenName) 
surname := "Bansky"
requestBody.SetSurname(&surname) 


typedEmailAddress := graphmodels.NewTypedEmailAddress()
additionalData := map[string]interface{}{
	"address" : "pavelb@contoso.onmicrosoft.com", 
	"name" : "Pavel Bansky", 
	"type" : "personal", 
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


phone := graphmodels.NewPhone()
number := "+1 732 555 0102"
phone.SetNumber(&number) 
type := graphmodels.BUSINESS_PHONETYPE 
phone.SetType(&type) 

phones := []graphmodels.Phoneable {
	phone,

}
requestBody.SetPhones(phones)

result, err := graphClient.Me().Contacts().Post(requestBody)


```