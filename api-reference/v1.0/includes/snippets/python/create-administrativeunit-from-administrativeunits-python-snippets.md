---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdministrativeUnit()
request_body.setDisplayName('Seattle District Technical Schools')

request_body.setDescription('Seattle district technical schools administration')

request_body.setVisibility('HiddenMembership')



result = await client.directory.administrativeUnits.post(request_body)


```