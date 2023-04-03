---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

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


requestConfiguration = GetScheduleRequestBuilderPostRequestConfiguration();

headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().calendar().getSchedule().post(requestBody, requestConfiguration);


```