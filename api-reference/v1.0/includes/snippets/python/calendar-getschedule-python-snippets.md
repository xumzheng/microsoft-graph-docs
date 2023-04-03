---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GetSchedulePostRequestBody();
requestBody.setSchedules(['adelev@contoso.onmicrosoft.com', 'meganb@contoso.onmicrosoft.com', ]);

startTime = DateTimeTimeZone();
startTime.setDateTime('2019-03-15T09:00:00');

startTime.setTimeZone('Pacific Standard Time');


requestBody.setStartTime($startTime);
endTime = DateTimeTimeZone();
endTime.setDateTime('2019-03-15T18:00:00');

endTime.setTimeZone('Pacific Standard Time');


requestBody.setEndTime($endTime);
requestBody.setAvailabilityViewInterval(60);


request_config = GetScheduleRequestBuilderPostRequestConfiguration();

headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

request_config.headers = headers;


result = await client.me().calendar().getSchedule().post(requestBody, request_config);


```