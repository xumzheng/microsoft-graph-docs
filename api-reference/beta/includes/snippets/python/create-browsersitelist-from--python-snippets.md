---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BrowserSiteList();
requestBody.setDisplayName('Production Site List A');

requestBody.setDescription('Production site list for team A');



requestResult = graphServiceClient.admin().edge().internetExplorerMode().siteLists().post(requestBody);


```