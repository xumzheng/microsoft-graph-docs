---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ContentType();
requestBody.setName('docSet');

requestBody.setDescription('custom docset');

base = ContentType();
base.setName('Document Set');

base.setId('0x0120D520');


requestBody.setBase($base);
requestBody.setGroup('Document Set Content Types');



result = awaitclient.sitesById('site-id').contentTypes().post(requestBody);


```