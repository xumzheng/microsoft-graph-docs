---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SetVerifiedPublisherPostRequestBody();
requestBody.setVerifiedPublisherId('1234567');



await client.applicationsById('application-id').setVerifiedPublisher().post(requestBody);


```