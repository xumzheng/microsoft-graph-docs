---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SetVerifiedPublisherPostRequestBody();
requestBody.setVerifiedPublisherId('1234567');



graphServiceClient.applicationsById('application-id').setVerifiedPublisher().post(requestBody);


```