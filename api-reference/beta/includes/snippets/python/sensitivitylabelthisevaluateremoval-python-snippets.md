---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EvaluateRemovalPostRequestBody()
content_info = ContentInfo()
contentInfo.@odatatype = '#microsoft.graph.security.contentInfo'

ContentInfo.identifier=null

contentInfo.State(ContentState('rest'))

metadata_key_value_pair1 = KeyValuePair()
metadataKeyValuePair1.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_Enabled'

metadataKeyValuePair1.value = 'True'


metadataArray []= metadataKeyValuePair1;
metadata_key_value_pair2 = KeyValuePair()
metadataKeyValuePair2.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_Method'

metadataKeyValuePair2.value = 'Standard'


metadataArray []= metadataKeyValuePair2;
metadata_key_value_pair3 = KeyValuePair()
metadataKeyValuePair3.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_SetDate'

metadataKeyValuePair3.value = '1/1/0001 12:00:00 AM'


metadataArray []= metadataKeyValuePair3;
metadata_key_value_pair4 = KeyValuePair()
metadataKeyValuePair4.@odatatype = '#microsoft.graph.security.keyValuePair'

metadataKeyValuePair4.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_SiteId'

metadataKeyValuePair4.value = 'cfa4cf1d-a337-4481-aa99-19d8f3d63f7c'


metadataArray []= metadataKeyValuePair4;
metadata_key_value_pair5 = KeyValuePair()
metadataKeyValuePair5.@odatatype = '#microsoft.graph.security.keyValuePair'

metadataKeyValuePair5.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_Name'

metadataKeyValuePair5.value = 'LabelScopedToBob_Tests'


metadataArray []= metadataKeyValuePair5;
metadata_key_value_pair6 = KeyValuePair()
metadataKeyValuePair6.@odatatype = '#microsoft.graph.security.keyValuePair'

metadataKeyValuePair6.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_ContentBits'

metadataKeyValuePair6.value = '0'


metadataArray []= metadataKeyValuePair6;
metadata_key_value_pair7 = KeyValuePair()
metadataKeyValuePair7.@odatatype = '#microsoft.graph.security.keyValuePair'

metadataKeyValuePair7.name = 'MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_ActionId'

metadataKeyValuePair7.value = '00000000-0000-0000-0000-000000000000'


metadataArray []= metadataKeyValuePair7;
contentInfo.metadata(metadataArray)



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


result = await client.users_by_id('user-id').security.informationProtection.sensitivityLabels.securityevaluateRemoval.post(request_body = request_body, request_configuration = request_configuration)


```