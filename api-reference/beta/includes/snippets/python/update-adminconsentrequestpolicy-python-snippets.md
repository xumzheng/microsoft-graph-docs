---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdminConsentRequestPolicyPutRequestBody()
additionalData = [
'isEnabled' => true,
'notifyReviewers' => true,
'remindersEnabled' => true,
'requestDurationInDays' => 5,
'reviewers' => reviewers1 = ()
		reviewers1.query = '/users/b6879be8-fb87-4482-a72e-18445d2b5c54'

		reviewers1.queryType = 'MicrosoftGraph'


reviewersArray []= reviewers1;
reviewers2 = ()
		reviewers2.query = '/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9'

		reviewers2.queryType = 'MicrosoftGraph'


reviewersArray []= reviewers2;
request_body.reviewers(reviewersArray)


];
request_body.additionaldata(additionalData)




request_configuration = AdminConsentRequestPolicyRequestBuilderPutRequestConfiguration(
)


await client.policies.adminConsentRequestPolicy.put(request_body = request_body)


```