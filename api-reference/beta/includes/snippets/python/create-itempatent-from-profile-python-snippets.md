---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemPatent()
request_body.setDescription('Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.')

request_body.setDisplayName('Inferring User Intent through browsing behaviors')

request_body.setIsPending(true)

request_body.setNumber('USPTO-3954432633')

request_body.setWebUrl('https://patents.gov/3954432633')


request_config = PatentsRequestBuilderPostRequestConfiguration(
request_config = PatentsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.profile.patents.post(request_body, headers=)


```