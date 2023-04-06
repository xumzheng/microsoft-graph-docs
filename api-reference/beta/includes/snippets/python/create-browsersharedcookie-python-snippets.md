---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSharedCookie()
request_body.set@odatatype('#microsoft.graph.browserSharedCookie')

request_body.setHostOrDomain('www.microsoft.com')

request_body.setSourceEnvironment(BrowserSharedCookieSourceEnvironment('internetexplorer11'))

request_body.setDisplayName('Microsoft Cookie')

request_body.setHostOnly(true)

request_body.setComment('A cookie for microsoft.com')

request_body.setPath('/')


request_config = SharedCookiesRequestBuilderPostRequestConfiguration(
request_config = SharedCookiesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').sharedCookies.post(request_body, headers=)


```