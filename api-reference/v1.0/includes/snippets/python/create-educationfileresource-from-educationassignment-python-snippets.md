---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.distribute_for_student_work = False

resource = EducationResource()
resource.displayName = 'article.pdf'

resource.@odatatype = '#microsoft.graph.educationFileResource'

additionalData = [
'file' => resource = File()
		resource.odataid = 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RPHKSP6THE4ORD2RQAR6MQLF26G'


resource.file = file

];
resource.additionaldata(additionalData)



request_body.resource = resource



result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').resources.post(request_body = request_body)


```