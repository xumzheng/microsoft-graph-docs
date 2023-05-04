---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Directory_setting()
request_body.template_id = '62375ab9-6b52-47ed-826b-58e47e0e304b'

values_setting_value1 = Setting_value()
values_setting_value1.name = 'GuestUsageGuidelinesUrl'

values_setting_value1.value = 'https://privacy.contoso.com/privacystatement'


valuesArray []= valuesSettingValue1;
values_setting_value2 = Setting_value()
values_setting_value2.name = 'EnableMSStandardBlockedWords'

values_setting_value2.value = 'true'


valuesArray []= valuesSettingValue2;
values_setting_value3 = Setting_value()
values_setting_value3.name = 'EnableMIPLabels'

values_setting_value3.value = 'true'


valuesArray []= valuesSettingValue3;
values_setting_value4 = Setting_value()
values_setting_value4.name = 'PrefixSuffixNamingRequirement'

values_setting_value4.value = '[Contoso-][GroupName]'


valuesArray []= valuesSettingValue4;
request_body.values(valuesArray)





result = await client.settings.post(request_body = request_body)


```