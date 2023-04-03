---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PrintTaskTrigger();
requestBody.setEvent(PrintEvent('jobstarted'));

additionalData = [
'definition@odata.bind' => 'https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c', 
];
requestBody.setAdditionalData(additionalData);




result = await client.print().printersById('printer-id').taskTriggers().post(requestBody);


```