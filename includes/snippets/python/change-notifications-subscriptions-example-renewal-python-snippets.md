---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Subscription()
request_body.setExpirationDateTime(DateTime('2016-03-22T11:00:00.0000000Z'))


request_config = SubscriptionRequestBuilderPatchRequestConfiguration(
request_config = SubscriptionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.subscriptions_by_id('subscription-id').patch(request_body, headers=)


```