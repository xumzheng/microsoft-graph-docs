---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DirectorySetting()
values_setting_value1 = SettingValue()
valuesSettingValue1.name = 'CustomBlockedWordsList'

valuesSettingValue1.value = 'Contoso'


valuesArray []= valuesSettingValue1;
request_body.values(valuesArray)





result = await client.settings_by_id('directorySetting-id').patch(request_body = request_body)


```