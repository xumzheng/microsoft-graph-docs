---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ColumnDefinition();
requestBody.setDescription('test');

requestBody.setEnforceUniqueValues(false);

requestBody.setHidden(false);

requestBody.setIndexed(false);

requestBody.setName('Title');

text = TextColumn();
text.setAllowMultipleLines(false);

text.setAppendChangesToExistingText(false);

text.setLinesForEditing(0);

text.setMaxLength(255);


requestBody.setText($text);


result = await client.sitesById('site-id').columns().post(requestBody);


```