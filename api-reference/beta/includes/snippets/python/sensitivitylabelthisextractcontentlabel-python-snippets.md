---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExtractContentLabelPostRequestBody()
contentInfo = ContentInfo()
contentInfo.identifier = 'MyDoc.docx'

contentInfo.State(ContentState('rest'))

metadataKeyValuePair1 = KeyValuePair()
metadataKeyValuePair1.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_Enabled'

metadataKeyValuePair1.value = 'True'


metadataArray []= metadataKeyValuePair1;
metadataKeyValuePair2 = KeyValuePair()
metadataKeyValuePair2.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_Method'

metadataKeyValuePair2.value = 'Standard'


metadataArray []= metadataKeyValuePair2;
metadataKeyValuePair3 = KeyValuePair()
metadataKeyValuePair3.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_SetDate'

metadataKeyValuePair3.value = '1/1/0001 12:00:00 AM'


metadataArray []= metadataKeyValuePair3;
metadataKeyValuePair4 = KeyValuePair()
metadataKeyValuePair4.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_SiteId'

metadataKeyValuePair4.value = 'cfa4cf1d-a337-4481-aa99-19d8f3d63f7c'


metadataArray []= metadataKeyValuePair4;
metadataKeyValuePair5 = KeyValuePair()
metadataKeyValuePair5.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_Name'

metadataKeyValuePair5.value = 'LabelScopedToBob_Tests'


metadataArray []= metadataKeyValuePair5;
metadataKeyValuePair6 = KeyValuePair()
metadataKeyValuePair6.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_ContentBits'

metadataKeyValuePair6.value = '0'


metadataArray []= metadataKeyValuePair6;
metadataKeyValuePair7 = KeyValuePair()
metadataKeyValuePair7.name = 'MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_ActionId'

metadataKeyValuePair7.value = '00000000-0000-0000-0000-000000000000'


metadataArray []= metadataKeyValuePair7;
contentInfo.metadata(metadataArray)


additionalData = [
'format' => 'default', 
];
contentInfo.additionaldata(additionalData)



request_body.contentInfo = contentInfo


request_configuration = ExtractContentLabelRequestBuilderPostRequestConfiguration(
headers = {
				'User-Agent' : "ContosoLOBApp/1.0",
}

)


result = await client.users_by_id('user-id').security.informationProtection.sensitivityLabels.securityextractContentLabel.post(request_body = request_body, request_configuration = request_configuration)


```