---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchemaPutRequestBody()
additionalData = [
'directories' => directories1 = ()
		directories1.setName('Azure Active Directory')

objects1 = ()
		objects1.setName('User')

attributes1 = ()
		attributes1.setName('userPrincipalName')

		attributes1.setType('string')


attributesArray []= attributes1;
objects1.setAttributes(attributesArray)



objectsArray []= objects1;
directories1.setObjects(objectsArray)



directoriesArray []= directories1;
directories2 = ()
directories2.setName('Salesforce')


directoriesArray []= directories2;
request_body.setDirectories(directoriesArray)


'synchronizationRules' => synchronizationRules1 = ()
synchronizationRules1.setName('USER_TO_USER')

synchronizationRules1.setSourceDirectoryName('Azure Active Directory')

synchronizationRules1.setTargetDirectoryName('Salesforce')

objectMappings1 = ()
objectMappings1.setSourceObjectName('User')

objectMappings1.setTargetObjectName('User')

attributeMappings1 = ()
attributeMappings1Source = Source()

attributeMappings1.setSource($attributeMappings1Source)
attributeMappings1.setTargetAttributeName('userName')


attributeMappingsArray []= attributeMappings1;
objectMappings1.setAttributeMappings(attributeMappingsArray)



objectMappingsArray []= objectMappings1;
synchronizationRules1.setObjectMappings(objectMappingsArray)



synchronizationRulesArray []= synchronizationRules1;
request_body.setSynchronizationRules(synchronizationRulesArray)


];
request_body.setAdditionalData(additionalData)




await client.servicePrincipalsById('servicePrincipal-id').synchronization.jobsById('synchronizationJob-id').schema.put(request_body)


```