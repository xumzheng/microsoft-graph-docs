---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new DirectorySetting();
$valuesSettingValue1 = new SettingValue();
$valuesSettingValue1.setName('CustomBlockedWordsList');

$valuesSettingValue1.setValue('Contoso');


$valuesArray []= $valuesSettingValue1;
$requestBody.setValues($valuesArray);




$requestResult = $graphServiceClient.settingsById('directorySetting-id').patch($requestBody);


```