---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OpenShift()
request_body.id = 'OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8'

request_body.schedulingGroupId = 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0'

sharedOpenShift = OpenShiftItem()
sharedOpenShift.notes = 'InventoryManagement'

sharedOpenShift.openSlotCount = 2

sharedOpenShift.displayName = 'Dayshift'

sharedOpenShift.startDateTime = DateTime('2018-10-04T00: 58: 45.340Z')

sharedOpenShift.endDateTime = DateTime('2018-10-04T09: 50: 45.332Z')

sharedOpenShift.Theme(ScheduleEntityTheme('white'))

activitiesShiftActivity1 = ShiftActivity()
activitiesShiftActivity1.isPaid = true

activitiesShiftActivity1.startDateTime = DateTime('2018-10-04T00: 58: 45.340Z')

activitiesShiftActivity1.endDateTime = DateTime('2018-10-04T01: 58: 45.340Z')

activitiesShiftActivity1.code = ''

activitiesShiftActivity1.displayName = 'Lunch'


activitiesArray []= activitiesShiftActivity1;
sharedOpenShift.activities(activitiesArray)



request_body.sharedOpenShift = sharedOpenShift
request_body.draftOpenShift=null

request_body.createdDateTime = DateTime('2019-03-14T04: 32: 51.451Z')

request_body.lastModifiedDateTime = DateTime('2019-03-14T05: 32: 51.451Z')

lastModifiedBy = IdentitySet()
LastModifiedBy.application=null

LastModifiedBy.device=null

lastModifiedByUser = Identity()
lastModifiedByUser.id = '366c0b19-49b1-41b5-a03f-9f3887bd0ed8'

lastModifiedByUser.displayName = 'JohnDoe'


lastModifiedBy.user = lastModifiedByUser
additionalData = [
'conversation' => 	null,
];
lastModifiedBy.additionaldata(additionalData)



request_body.lastModifiedBy = lastModifiedBy

headers = {
	'Authorization' : "Bearer {token}",
}

)


result = await client.teams_by_id('team-id').schedule.openShifts.post(request_body = request_body, request_configuration = request_configuration)


```