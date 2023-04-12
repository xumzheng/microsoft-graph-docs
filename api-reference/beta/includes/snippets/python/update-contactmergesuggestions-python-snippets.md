---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactMergeSuggestions()
request_body.isEnabled = false




result = await client.me.settings.contactMergeSuggestions.patch(request_body = request_body)


```