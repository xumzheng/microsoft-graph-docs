---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Bookmark();
requestBody.setDescription('Book a fancy vacation in Tuscany or browse museums in Florence.');



result = awaitclient.search().bookmarksById('bookmark-id').patch(requestBody);


```