---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BrowserSiteList();
requestBody.setDisplayName('Production Site List A');

requestBody.setDescription('Production site list for team A');



result = awaitclient.admin().edge().internetExplorerMode().siteLists().post(requestBody);


```