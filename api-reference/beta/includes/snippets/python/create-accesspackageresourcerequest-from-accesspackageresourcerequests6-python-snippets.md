---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.catalogId = '26ac0c0a-08bc-4a7b-a313-839f58044ba5'

request_body.requestType = 'AdminAdd'

request_body.justification = ''

access_package_resource = AccessPackageResource()
accessPackageResource.displayName = 'Faculty cafeteria ordering'

accessPackageResource.description = 'Example application'

accessPackageResource.url = 'https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/'

accessPackageResource.resourceType = 'Application'

accessPackageResource.originId = '2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e'

accessPackageResource.originSystem = 'AadApplication'

attributes_access_package_resource_attribute1 = AccessPackageResourceAttribute()
attributesAccessPackageResourceAttribute1.attributeName = 'extension_2b676109c7c74ae2b41549205f1947ed_personalTitle'

attributesAccessPackageResourceAttribute1.is_editable = True

attributesAccessPackageResourceAttribute1.is_persisted_on_assignment_removal = True

attributes_access_package_resource_attribute1_attribute_source = AccessPackageResourceAttributeSource()
attributesAccessPackageResourceAttribute1AttributeSource.@odatatype = '#microsoft.graph.accessPackageResourceAttributeQuestion'

additionalData = [
'question' => attributes_access_package_resource_attribute1_attribute_source = Question()
		attributesAccessPackageResourceAttribute1AttributeSource.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

		attributesAccessPackageResourceAttribute1AttributeSource.is_required = False

		attributesAccessPackageResourceAttribute1AttributeSource.sequence = 0

		attributesAccessPackageResourceAttribute1AttributeSource.is_single_line_question = True

text = Text()
		text.defaultText = 'Title'

text.LocalizedTexts([])


attributesAccessPackageResourceAttribute1AttributeSource.text = text

attributesAccessPackageResourceAttribute1AttributeSource.question = question

];
attributesAccessPackageResourceAttribute1AttributeSource.additionaldata(additionalData)



attributesAccessPackageResourceAttribute1.attribute_source = attributesAccessPackageResourceAttribute1AttributeSource
attributes_access_package_resource_attribute1_attribute_destination = AccessPackageResourceAttributeDestination()
attributesAccessPackageResourceAttribute1AttributeDestination.@odatatype = '#microsoft.graph.accessPackageUserDirectoryAttributeStore'


attributesAccessPackageResourceAttribute1.attribute_destination = attributesAccessPackageResourceAttribute1AttributeDestination

attributesArray []= attributesAccessPackageResourceAttribute1;
accessPackageResource.attributes(attributesArray)



request_body.access_package_resource = accessPackageResource



result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body = request_body)


```