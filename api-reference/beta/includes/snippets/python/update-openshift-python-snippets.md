---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OpenShift()
additionalData = [
'schedulingGroupId' => 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0', 
'sharedOpenShift' => request_body = SharedOpenShift()
		request_body.notes = 'Inventory Management'

		request_body.open_slot_count = 5

		request_body.displayName = 'Field shift'

		request_body.startDateTime = '2018-10-04T00:58:45.340Z'

		request_body.endDateTime = '2018-10-04T09:50:45.332Z'

		request_body.theme = 'white'

activities1 = ()
		activities1.is_paid = True

		activities1.startDateTime = '2018-10-04T00:58:45.340Z'

		activities1.endDateTime = '2018-10-04T01:58:45.340Z'

		activities1.code = ''

		activities1.displayName = 'Lunch'


activitiesArray []= activities1;
request_body.activities(activitiesArray)



request_body.shared_open_shift = sharedOpenShift

'draftOpenShift' => 	null,
];
request_body.additionaldata(additionalData)





await client.teams_by_id('team-id').schedule.openShifts_by_id('openShift-id').put(request_body = request_body)


```