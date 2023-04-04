---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SetVerifiedPublisherPostRequestBody();
request_body.setVerifiedPublisherId('1234567');



await client.applicationsById('application-id').setVerifiedPublisher().post(request_body);


```