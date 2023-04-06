---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IndustryDataConnector()
request_body.set@odatatype('#microsoft.graph.industryData.azureDataLakeConnector')

request_body.setDisplayName('CSV connector')

additionalData = [
'sourceSystem@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/sourceSystems(\'aa050107-5784-4a8e-1876-08daddab21bc\')', 
];
request_body.setAdditionalData(additionalData)



request_config = DataConnectorsRequestBuilderPostRequestConfiguration(
request_config = DataConnectorsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.external.industryData.dataConnectors.post(request_body, headers=)


```