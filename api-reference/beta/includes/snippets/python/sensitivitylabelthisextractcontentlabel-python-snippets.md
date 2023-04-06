---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExtractContentLabelPostRequestBody()
contentInfo = ContentInfo()
contentInfo.setIdentifier('MyDoc.docx')

contentInfo.setState(ContentState('rest'))

metadataKeyValuePair1 = KeyValuePair()
metadataKeyValuePair1.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_Enabled')

metadataKeyValuePair1.setValue('True')


metadataArray []= metadataKeyValuePair1;
metadataKeyValuePair2 = KeyValuePair()
metadataKeyValuePair2.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_Method')

metadataKeyValuePair2.setValue('Standard')


metadataArray []= metadataKeyValuePair2;
metadataKeyValuePair3 = KeyValuePair()
metadataKeyValuePair3.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_SetDate')

metadataKeyValuePair3.setValue('1/1/0001 12:00:00 AM')


metadataArray []= metadataKeyValuePair3;
metadataKeyValuePair4 = KeyValuePair()
metadataKeyValuePair4.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_SiteId')

metadataKeyValuePair4.setValue('cfa4cf1d-a337-4481-aa99-19d8f3d63f7c')


metadataArray []= metadataKeyValuePair4;
metadataKeyValuePair5 = KeyValuePair()
metadataKeyValuePair5.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_Name')

metadataKeyValuePair5.setValue('LabelScopedToBob_Tests')


metadataArray []= metadataKeyValuePair5;
metadataKeyValuePair6 = KeyValuePair()
metadataKeyValuePair6.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_ContentBits')

metadataKeyValuePair6.setValue('0')


metadataArray []= metadataKeyValuePair6;
metadataKeyValuePair7 = KeyValuePair()
metadataKeyValuePair7.setName('MSIP_Label_0ed12617-d0ef-4053-b8e4-ecf5bcf2ffb3_ActionId')

metadataKeyValuePair7.setValue('00000000-0000-0000-0000-000000000000')


metadataArray []= metadataKeyValuePair7;
contentInfo.setMetadata(metadataArray)


additionalData = [
'format' => 'default', 
];
contentInfo.setAdditionalData(additionalData)



request_body.setContentInfo($contentInfo)

request_config = ExtractContentLabelRequestBuilderPostRequestConfiguration(
request_config = ExtractContentLabelRequestBuilderPostRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.users_by_id('user-id').security.informationProtection.sensitivityLabels.securityextractContentLabel.post(request_body, request_config, headers=request_config)


```