---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/education/users/13015')


request_config = RefRequestBuilderPostRequestConfiguration(
request_config = RefRequestBuilderPostRequestConfiguration(query_params=)


await client.education.classes_by_id('educationClass-id').members.ref.post(request_body, headers=)


```