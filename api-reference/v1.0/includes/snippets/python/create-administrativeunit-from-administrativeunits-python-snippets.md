---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AdministrativeUnit();
requestBody.setDisplayName('Seattle District Technical Schools');

requestBody.setDescription('Seattle district technical schools administration');

requestBody.setVisibility('HiddenMembership');



result = await client.directory().administrativeUnits().post(requestBody);


```