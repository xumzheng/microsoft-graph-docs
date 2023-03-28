---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GroupSetting();
$valuesSettingValue1 = new SettingValue();
$valuesSettingValue1.setName('AllowToAddGuests');

$valuesSettingValue1.setValue('false');


$valuesArray []= $valuesSettingValue1;
$requestBody.setValues($valuesArray);




$requestResult = $graphServiceClient.groupSettingsById('groupSetting-id').patch($requestBody);


```