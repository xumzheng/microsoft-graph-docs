---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EvaluateApplicationPostRequestBody()
contentInfo = ContentInfo()
contentInfo.@odatatype = '#microsoft.graph.contentInfo'

contentInfo.Format(ContentFormat('default'))

ContentInfo.identifier=null

contentInfo.State(ContentState('rest'))

metadataKeyValuePair1 = KeyValuePair()
metadataKeyValuePair1.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair1.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled'

metadataKeyValuePair1.value = 'True'


metadataArray []= metadataKeyValuePair1;
metadataKeyValuePair2 = KeyValuePair()
metadataKeyValuePair2.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair2.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method'

metadataKeyValuePair2.value = 'Standard'


metadataArray []= metadataKeyValuePair2;
metadataKeyValuePair3 = KeyValuePair()
metadataKeyValuePair3.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair3.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate'

metadataKeyValuePair3.value = '1/1/0001 12:00:00 AM'


metadataArray []= metadataKeyValuePair3;
metadataKeyValuePair4 = KeyValuePair()
metadataKeyValuePair4.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair4.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId'

metadataKeyValuePair4.value = 'cfa4cf1d-a337-4481-aa99-19d8f3d63f7c'


metadataArray []= metadataKeyValuePair4;
metadataKeyValuePair5 = KeyValuePair()
metadataKeyValuePair5.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair5.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name'

metadataKeyValuePair5.value = 'General'


metadataArray []= metadataKeyValuePair5;
metadataKeyValuePair6 = KeyValuePair()
metadataKeyValuePair6.@odatatype = '#microsoft.graph.keyValuePair'

metadataKeyValuePair6.name = 'MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits'

metadataKeyValuePair6.value = '0'


metadataArray []= metadataKeyValuePair6;
metadataKeyValuePair7 = KeyValuePair()
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



request_body.contentInfo = contentInfo
labelingOptions = LabelingOptions()
labelingOptions.@odatatype = '#microsoft.graph.labelingOptions'

labelingOptions.AssignmentMethod(AssignmentMethod('standard'))

labelingOptions.labelId = '97309856-9c28-4ac6-9382-5f8bc20c457b'

LabelingOptions.downgradeJustification=null

labelingOptions.ExtendedProperties([])

additionalData = [
'assignmentMethod@odata.type' => '#microsoft.graph.assignmentMethod', 
'labelId@odata.type' => '#Guid', 
'extendedProperties@odata.type' => '#Collection(microsoft.graph.keyValuePair)', 
];
labelingOptions.additionaldata(additionalData)



request_body.labelingOptions = labelingOptions



result = await client.informationProtection.policy.labels.evaluateApplication.post(request_body = request_body, request_configuration = request_configuration)


```