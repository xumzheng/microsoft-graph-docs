---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetVerifiedPublisherPostRequestBody()
request_body.verifiedPublisherId = '1234567'



request_configuration = SetVerifiedPublisherRequestBuilderPostRequestConfiguration(
)


await client.applications_by_id('application-id').setVerifiedPublisher.post(request_body = request_body)


```