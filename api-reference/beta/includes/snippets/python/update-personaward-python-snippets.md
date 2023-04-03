---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonAward();
requestBody.setIssuingAuthority('International Association of Branding Management');

requestBody.setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');



result = awaitclient.usersById('user-id').profile().awardsById('personAward-id').patch(requestBody);


```