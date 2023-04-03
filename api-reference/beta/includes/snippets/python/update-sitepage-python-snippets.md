---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SitePage();
requestBody.set@odatatype('#microsoft.graph.sitePage');

requestBody.setTitle('sample');

requestBody.setShowComments(true);

requestBody.setShowRecommendedPages(false);



result = await client.sitesById('site-id').pagesById('sitePage-id').patch(requestBody);


```