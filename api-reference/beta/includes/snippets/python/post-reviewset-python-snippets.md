---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReviewSet()
request_body.setDisplayName('My Reviewset 3')



result = await client.compliance.ediscovery.casesById('case-id').reviewSets.post(request_body)


```