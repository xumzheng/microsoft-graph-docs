---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.distributeForStudentWork = false

resource = EducationResource()
resource.displayName = 'Template - My Story'

resource.@odatatype = '#microsoft.graph.educationTeamsAppResource'

additionalData = [
'appId' => '6fbeb90c-3d55-4bd5-82c4-bfe824be4300', 
'appIconWebUrl' => 'https://statics.teams.cdn.office.net/evergreen-assets/ThirdPartyApps/6fbeb90c-3d55-4bd5-82c4-bfe824be4300_largeImage.png?v=2.0.2', 
'teamsEmbeddedContentUrl' => 'https://app.api.edu.buncee.com/player/C7B0866C9B7E485EAE21AE14DBC3FD08?embed=1&render_slide_panel=1', 
'webUrl' => 'https://app.edu.buncee.com/buncee/C7B0866C9B7E485EAE21AE14DBC3FD08', 
];
resource.additionaldata(additionalData)



request_body.resource = resource



result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').resources.post(request_body = request_body)


```