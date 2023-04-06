---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/beta/education/users/14008')


request_config = RefRequestBuilderPostRequestConfiguration(
request_config = RefRequestBuilderPostRequestConfiguration(query_params=)


await client.education.schools_by_id('educationSchool-id').users.ref.post(request_body, headers=)


```