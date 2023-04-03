---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BrowserSharedCookie();
requestBody.set@odatatype('#microsoft.graph.browserSharedCookie');

requestBody.setHostOrDomain('www.microsoft.com');

requestBody.setSourceEnvironment(BrowserSharedCookieSourceEnvironment('internetexplorer11'));

requestBody.setDisplayName('Microsoft Cookie');

requestBody.setHostOnly(true);

requestBody.setComment('A cookie for microsoft.com');

requestBody.setPath('/');



result = await client.admin().edge().internetExplorerMode().siteListsById('browserSiteList-id').sharedCookies().post(requestBody);


```