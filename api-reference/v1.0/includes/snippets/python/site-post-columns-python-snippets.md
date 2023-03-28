---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ColumnDefinition();
$requestBody.setDescription('test');

$requestBody.setEnforceUniqueValues(false);

$requestBody.setHidden(false);

$requestBody.setIndexed(false);

$requestBody.setName('Title');

$text = new TextColumn();
$text.setAllowMultipleLines(false);

$text.setAppendChangesToExistingText(false);

$text.setLinesForEditing(0);

$text.setMaxLength(255);


$requestBody.setText($text);


$requestResult = $graphServiceClient.sitesById('site-id').columns().post($requestBody);


```