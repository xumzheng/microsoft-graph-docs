---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdministrativeUnit()
request_body.setDisplayName('Greater Seattle District Technical Schools')



result = await client.directory.administrativeUnits._by_id('administrativeUnit-id').patch(request_body)


```