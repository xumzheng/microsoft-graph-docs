---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSubmissionResource()
resource = EducationResource()
resource.setDisplayName('category.jpg')

resource.set@odatatype('#microsoft.graph.educationMediaResource')

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)


result = await client.education.classes._by_id('educationClass-id').assignments._by_id('educationAssignment-id').submissions._by_id('educationSubmission-id').resources.post(request_body)


```