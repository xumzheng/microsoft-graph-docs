---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PersonAward();
request_body.setIssuingAuthority('International Association of Branding Management');

request_body.setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');



result = await client.usersById('user-id').profile().awardsById('personAward-id').patch(request_body);


```