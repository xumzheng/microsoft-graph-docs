---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AdministrativeUnit();
requestBody.setDisplayName('Greater Seattle District Technical Schools');



result = awaitclient.directory().administrativeUnitsById('administrativeUnit-id').patch(requestBody);


```