---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PersonWebsite()
request_body.Categories(['football', ])

request_body.displayName = 'Lyn Damer'

request_body.webUrl = 'www.lyndamer.no'



request_configuration = WebsitesRequestBuilderPostRequestConfiguration(
)


result = await client.me.profile.websites.post(request_body = request_body)


```