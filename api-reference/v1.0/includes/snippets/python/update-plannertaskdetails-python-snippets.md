---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerTaskDetails()
request_body.setPreviewType(PlannerPreviewType('nopreview'))

references = PlannerExternalReferences()
additionalData = [
'http%3A//developer%2Emicrosoft%2Ecom' => references = Http%3A//developer%2Emicrosoft%2Ecom()
		references.set@odatatype('microsoft.graph.plannerExternalReference')

		references.setAlias('Documentation')

		references.setPreviewPriority(' !')

		references.setType('Other')


references.setHttp%3A//developer%2Emicrosoft%2Ecom($http%3A//developer%2Emicrosoft%2Ecom)

'https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer' => references = Https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer()
		references.set@odatatype('microsoft.graph.plannerExternalReference')

		references.setPreviewPriority('  !!')


references.setHttps%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer($https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer)

'http%3A//www%2Ebing%2Ecom' => 		null,
];
references.setAdditionalData(additionalData)



request_body.setReferences($references)
checklist = PlannerChecklistItems()
additionalData = [
'95e27074-6c4a-447a-aa24-9d718a0b86fa' => checklist = 95e27074-6c4a-447a-aa24-9d718a0b86fa()
		checklist.set@odatatype('microsoft.graph.plannerChecklistItem')

		checklist.setTitle('Update task details')

		checklist.setIsChecked(true)


checklist.set95e27074-6c4a-447a-aa24-9d718a0b86fa($95e27074-6c4a-447a-aa24-9d718a0b86fa)

'd280ed1a-9f6b-4f9c-a962-fb4d00dc50ff' => checklist = D280ed1a-9f6b-4f9c-a962-fb4d00dc50ff()
		checklist.set@odatatype('microsoft.graph.plannerChecklistItem')

		checklist.setIsChecked(true)


checklist.setD280ed1a-9f6b-4f9c-a962-fb4d00dc50ff($d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff)

'a93c93c5-10a6-4167-9551-8bafa09967a7' => 		null,
];
checklist.setAdditionalData(additionalData)



request_body.setChecklist($checklist)

request_config = DetailsRequestBuilderPatchRequestConfiguration(
request_config = DetailsRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"
headers['If-Match'] = "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""


result = await client.planner.tasks_by_id('plannerTask-id').details.patch(request_body, request_config, headers=request_config)


```