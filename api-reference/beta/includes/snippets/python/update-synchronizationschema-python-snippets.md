---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchemaPutRequestBody()
additionalData = [
'directories' => directories1 = ()
		directories1.name = 'Azure Active Directory'

objects1 = ()
		objects1.name = 'User'

attributes1 = ()
		attributes1.name = 'userPrincipalName'

		attributes1.type = 'string'


attributesArray []= attributes1;
objects1.attributes(attributesArray)



objectsArray []= objects1;
directories1.objects(objectsArray)



directoriesArray []= directories1;
directories2 = ()
directories2.name = 'Salesforce'


directoriesArray []= directories2;
request_body.directories(directoriesArray)


'synchronizationRules' => synchronization_rules1 = ()
synchronizationRules1.name = 'USER_TO_USER'

synchronizationRules1.sourceDirectoryName = 'Azure Active Directory'

synchronizationRules1.targetDirectoryName = 'Salesforce'

object_mappings1 = ()
objectMappings1.sourceObjectName = 'User'

objectMappings1.targetObjectName = 'User'

attribute_mappings1 = ()
attribute_mappings1_source = Source()

attributeMappings1.source = attributeMappings1Source
attributeMappings1.targetAttributeName = 'userName'


attributeMappingsArray []= attributeMappings1;
objectMappings1.attributemappings(attributeMappingsArray)



objectMappingsArray []= objectMappings1;
synchronizationRules1.objectmappings(objectMappingsArray)



synchronizationRulesArray []= synchronizationRules1;
request_body.synchronizationrules(synchronizationRulesArray)


];
request_body.additionaldata(additionalData)





await client.servicePrincipals_by_id('servicePrincipal-id').synchronization.jobs_by_id('synchronizationJob-id').schema.put(request_body = request_body)


```