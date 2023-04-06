---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSharedCookie()
request_body.setHostOrDomain('www.microsoft.com')

request_body.setSourceEnvironment(BrowserSharedCookieSourceEnvironment('microsoftedge'))

request_body.setDisplayName('Microsoft Cookie')

request_body.setPath('/')

request_body.setHostOnly(true)

request_body.setComment('Updating source environment.')


request_config = BrowserSharedCookieRequestBuilderPatchRequestConfiguration(
request_config = BrowserSharedCookieRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').sharedCookies_by_id('browserSharedCookie-id').patch(request_body, headers=)


```