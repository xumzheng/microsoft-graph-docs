---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPhone()
request_body.setDisplayName('Car Phone')

request_body.setNumber('+7 499 342 22 13')


request_config = PhonesRequestBuilderPostRequestConfiguration(
request_config = PhonesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.profile.phones.post(request_body, headers=)


```