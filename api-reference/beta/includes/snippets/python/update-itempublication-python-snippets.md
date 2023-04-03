---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ItemPublication();
requestBody.setPublisher('International Association of Branding Management Publishing');

requestBody.setThumbnailUrl('https://iabm.io/sdhdfhsdhshsd.jpg');



requestResult = graphServiceClient.usersById('user-id').profile().publicationsById('itemPublication-id').patch(requestBody);


```