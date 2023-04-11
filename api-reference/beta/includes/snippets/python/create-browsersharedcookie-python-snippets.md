---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSharedCookie()
request_body.@odatatype = '#microsoft.graph.browserSharedCookie'

request_body.hostOrDomain = 'www.microsoft.com'

request_body.SourceEnvironment(BrowserSharedCookieSourceEnvironment('internetexplorer11'))

request_body.displayName = 'Microsoft Cookie'

request_body.hostOnly = true

request_body.comment = 'A cookie for microsoft.com'

request_body.path = '/'



request_configuration = SharedCookiesRequestBuilderPostRequestConfiguration(
)


result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').sharedCookies.post(request_body = request_body)


```