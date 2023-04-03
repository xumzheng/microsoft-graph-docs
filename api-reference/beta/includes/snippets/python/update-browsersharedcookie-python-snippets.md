---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BrowserSharedCookie();
requestBody.setHostOrDomain('www.microsoft.com');

requestBody.setSourceEnvironment(BrowserSharedCookieSourceEnvironment('microsoftedge'));

requestBody.setDisplayName('Microsoft Cookie');

requestBody.setPath('/');

requestBody.setHostOnly(true);

requestBody.setComment('Updating source environment.');



result = awaitclient.admin().edge().internetExplorerMode().siteListsById('browserSiteList-id').sharedCookiesById('browserSharedCookie-id').patch(requestBody);


```