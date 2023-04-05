---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContentType()
request_body.setName('docSet')

request_body.setDescription('custom docset')

base = ContentType()
base.setName('Document Set')

base.setId('0x0120D520')


request_body.setBase($base)
request_body.setGroup('Document Set Content Types')



result = await client.sitesById('site-id').contentTypes.post(request_body)


```