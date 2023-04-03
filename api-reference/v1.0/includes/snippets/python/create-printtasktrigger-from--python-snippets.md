---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PrintTaskTrigger();
requestBody.setEvent(PrintEvent('jobstarted'));

additionalData = [
'definition@odata.bind' => 'https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}', 
];
requestBody.setAdditionalData(additionalData);




result = await client.print().printersById('printer-id').taskTriggers().post(requestBody);


```