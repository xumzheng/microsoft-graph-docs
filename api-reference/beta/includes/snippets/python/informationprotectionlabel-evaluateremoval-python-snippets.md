---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EvaluateRemovalPostRequestBody()
content_info = ContentInfo()
contentInfo.@odatatype = '#microsoft.graph.contentInfo'

contentInfo.Format(ContentFormat('default'))

ContentInfo.identifier=null

contentInfo.State(ContentState('rest'))

metadata_key_value_pair1 = KeyValuePair()
metadataKeyValuePair1.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair1.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled'

metadataKeyValuePair1.value = 'True'


metadataArray []= metadataKeyValuePair1;
metadata_key_value_pair2 = KeyValuePair()
metadataKeyValuePair2.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair2.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method'

metadataKeyValuePair2.value = 'Standard'


metadataArray []= metadataKeyValuePair2;
metadata_key_value_pair3 = KeyValuePair()
metadataKeyValuePair3.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair3.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate'

metadataKeyValuePair3.value = '1/1/0001 12:00:00 AM'


metadataArray []= metadataKeyValuePair3;
metadata_key_value_pair4 = KeyValuePair()
metadataKeyValuePair4.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair4.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId'

metadataKeyValuePair4.value = 'cfa4cf1d-a337-4481-aa99-19d8f3d63f7c'


metadataArray []= metadataKeyValuePair4;
metadata_key_value_pair5 = KeyValuePair()
metadataKeyValuePair5.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair5.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name'

metadataKeyValuePair5.value = 'General'


metadataArray []= metadataKeyValuePair5;
metadata_key_value_pair6 = KeyValuePair()
metadataKeyValuePair6.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair6.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits'

metadataKeyValuePair6.value = '0'


metadataArray []= metadataKeyValuePair6;
metadata_key_value_pair7 = KeyValuePair()
metadataKeyValuePair7.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair7.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId'

metadataKeyValuePair7.value = '00000000-0000-0000-0000-000000000000'


metadataArray []= metadataKeyValuePair7;
contentInfo.metadata(metadataArray)


additionalData = [
'format@odata.type' => '#microsoft.graph.contentFormat', 
'state@odata.type' => '#microsoft.graph.contentState', 
'metadata@odata.type' => '#Collection(microsoft.graph.keyValuePair)', 
];
contentInfo.additionaldata(additionalData)



request_body.content_info = contentInfo
downgrade_justification = DowngradeJustification()
downgradeJustification.justificationMessage = 'The information has been declassified.'

downgradeJustification.is_downgrade_justified = True


request_body.downgrade_justification = downgradeJustification


request_configuration = EvaluateRemovalRequestBuilder.EvaluateRemovalRequestBuilderPostRequestConfiguration(
headers = {
	'User-Agent' : "ContosoLOBApp/1.0",
}

)


result = await client.informationProtection.policy.labels.evaluateRemoval.post(request_body = request_body, request_configuration = request_configuration)


```