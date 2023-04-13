---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Shift()
additionalData = [
'id' => 'SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8', 
'createdDateTime' => '2019-03-14T04:32:51.451Z', 
'lastModifiedDateTime' => '2019-03-14T05:32:51.451Z', 
'userId' => 'c5d0c76b-80c4-481c-be50-923cd8d680a1', 
'schedulingGroupId' => 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0', 
'lastModifiedBy' => request_body = LastModifiedBy()
		request_body.application=null

		request_body.device=null

		request_body.conversation=null

user = User()
		user.id = '366c0b19-49b1-41b5-a03f-9f3887bd0ed8'

		user.displayName = 'John Doe'


request_body.user = user

request_body.lastModifiedBy = lastModifiedBy

'sharedShift' => request_body = SharedShift()
		request_body.displayName = 'Day shift'

		request_body.notes = 'Please do inventory as part of your shift.'

		request_body.startDateTime = '2019-03-11T15:00:00Z'

		request_body.endDateTime = '2019-03-12T00:00:00Z'

		request_body.theme = 'blue'

activities1 = ()
		activities1.isPaid = true

		activities1.startDateTime = '2019-03-11T15:00:00Z'

		activities1.endDateTime = '2019-03-11T15:15:00Z'

		activities1.code = ''

		activities1.displayName = 'Lunch'


activitiesArray []= activities1;
request_body.activities(activitiesArray)



request_body.sharedShift = sharedShift

'draftShift' => request_body = DraftShift()
	request_body.displayName = 'Day shift'

	request_body.notes = 'Please do inventory as part of your shift.'

	request_body.startDateTime = '2019-03-11T15:00:00Z'

	request_body.endDateTime = '2019-03-12T00:00:00Z'

	request_body.theme = 'blue'

activities1 = ()
	activities1.isPaid = true

	activities1.startDateTime = '2019-03-11T15:00:00Z'

	activities1.endDateTime = '2019-03-11T15:30:00Z'

	activities1.code = ''

	activities1.displayName = 'Lunch'


activitiesArray []= activities1;
request_body.activities(activitiesArray)



request_body.draftShift = draftShift

];
request_body.additionaldata(additionalData)





await client.teams_by_id('team-id').schedule.shifts_by_id('shift-id').put(request_body = request_body, request_configuration = request_configuration)


```