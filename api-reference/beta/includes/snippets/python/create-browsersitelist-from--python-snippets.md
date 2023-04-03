---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BrowserSiteList();
requestBody.setDisplayName('Production Site List A');

requestBody.setDescription('Production site list for team A');



result = await client.admin().edge().internetExplorerMode().siteLists().post(requestBody);


```