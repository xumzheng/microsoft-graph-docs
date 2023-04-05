---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GroupSetting()
valuesSettingValue1 = SettingValue()
valuesSettingValue1.setName('AllowToAddGuests')

valuesSettingValue1.setValue('true')


valuesArray []= valuesSettingValue1;
request_body.setValues(valuesArray)




result = await client.groupsby_id('group-id')_settingsby_id('groupSetting-id').patch(request_body)


```