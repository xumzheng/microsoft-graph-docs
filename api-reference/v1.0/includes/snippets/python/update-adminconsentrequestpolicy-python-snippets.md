---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AdminConsentRequestPolicyPutRequestBody();
additionalData = [
'isEnabled' => true,
'notifyReviewers' => true,
'remindersEnabled' => true,
'requestDurationInDays' => 5,
'reviewers' => reviewers1 = ();
		reviewers1.setQuery('/users/b6879be8-fb87-4482-a72e-18445d2b5c54');

		reviewers1.setQueryType('MicrosoftGraph');


reviewersArray []= reviewers1;
reviewers2 = ();
		reviewers2.setQuery('/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9');

		reviewers2.setQueryType('MicrosoftGraph');


reviewersArray []= reviewers2;
requestBody.setReviewers(reviewersArray);


];
requestBody.setAdditionalData(additionalData);




graphServiceClient.policies().adminConsentRequestPolicy().put(requestBody);


```