---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = LegalHold()
request_body.setDescription('This is a description for a legalHold')



result = await client.compliance.ediscovery.casesById('case-id').legalHoldsById('legalHold-id').patch(request_body)


```