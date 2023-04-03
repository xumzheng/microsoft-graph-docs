---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AdministrativeUnit();
requestBody.setDisplayName('Greater Seattle District Technical Schools');



requestResult = graphServiceClient.directory().administrativeUnitsById('administrativeUnit-id').patch(requestBody);


```