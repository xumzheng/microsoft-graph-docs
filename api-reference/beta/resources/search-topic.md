---
title: "topic resource type"
description: "Represents a topic in Microsoft Search."
author: "yijit-msft"
ms.localizationpriority: medium
ms.prod: "search"
doc_type: resourcePageType
---

# qna resource type

Namespace: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A topic represents a Viva Topic, which uses AI to automatically search for and identify topics in an organzation. It compiles information about them, such as a short description, people working on the topic, and sites, files, and pages that are related to it. 

## Methods

|Method|Return type|Description|
|:---|:---|:---|
|[Get topic](../api/search-topic-get.md)|[microsoft.graph.search.topic](../resources/search-topic.md)|Read the properties and relationships of a [topic](../resources/search-topic.md) object.|

## Properties

|Property|Type|Description|
|:---|:---|:---|
| id (inherited) | Edm.String | The unique identifier of the topic. |
| primaryName | microsoft.graph.topicName | The object representing the most relevant name and its metadata. | 
| alternateNames | Collection(microsoft.graph.topicName) | A list of objects representing all other relevant names and their metadata. | 
| definition | microsoft.graph.topicDefinition | The object representing a short description of the topic. | 
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the topic, whether a topic is suggested, confirmed, or published. | 
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the topic. The data includes the user's feedback on the topic item. | 
| webUrl | Edm.String | The URL of the topic directing viewer to the topic page in SharePoint topic center. | 
| currentLanguagueTag | Edm.String | The language tag of the current topic view |
| languageInfos | Collection(microsoft.graph.topicLanguageInfo) | Other available language infos of the current topic, with language name and the URL to visit topic page using given language. | 
| highlyRelatedFiles | Collection(microsoft.graph.topicFile) | The list hosting at most 10 files mined or curated that are highly relevant for this topic. |
| highlyRelatedSites | Collection(microsoft.graph.topicSite) | The list hosting at most 10 sites mined or curated that are highly relevant for this topic. |
| highlyRelatedUsers | Collection(microsoft.graph.topicUser) | The list hosting at most 10 users mined or curated that are highly relevant for this topic. |
| lastModifiedBy | microsoft.graph.identity | The last modifier of the topic, if the topic has been modified | 
| lastModifiedDateTime | Edm.DateTimeOffset | The last modified time of the topic, if the topic has been modified | 

## Types
### View point

Represents user viewpoints data on the topic. The data includes the user's feedback on the topic item

| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| personalFeedbackState | microsoft.graph.topicPersonalFeedbackState | The feedback state current user has given to the topic name, whether a topic is confirmed, excluded, or unspecified for current user. |

### Enum: topicPersonalFeedbackState

```xml
<EnumType Name="topicPersonalFeedbackState">
    <Member Name="unspecified" Value="0" />
    <Member Name="confirmed" Value="1" />
    <Member Name="excluded" Value="2" />
    <Member Name="unknownFutureValue" Value="3" />
</EnumType>
```

### Lifecycle
The lifecycle represents the state of a topic, or a resource related to the topic. Based on whether a topic is mined or curated, or a topic is confirmed or removed, either by user, or by knowledge administrators.

#### Properties
| Property       | Type           | Description                                 |
| -------------- | -------------- | ------------------------------------------- |
| state | microsoft.graph.topicLifecycleState | The lifecycle state enum type. | No | Yes | Yes |
| lastModifiedDateTime | Edm.DateTimeOffset | The last modified time of the lifecycle, if the lifecycle has been modified | No | No | Yes |


### Enum: topicLifecycleState
```xml
<EnumType Name="topicLifecycleState">
    <Member Name="suggested" Value="0" />
    <Member Name="confirmed" Value="1" />
    <Member Name="published" Value="2" />
    <Member Name="removed" Value="3" />
    <Member Name="unknownFutureValue" Value="4" />
</EnumType>
```

### Language Info
Language info represents the language available for a topic, and the URL redirect the user to the topic page containing topic metadata for the given language.

#### Properties

| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| value | Edm.String | The language code (ISO 639-1). | 
| webUrl | Edm.String | The URL for the topic page with metadata showing in the given language code | 

### Topic Resource Base
The base resource related to a topic.

#### Properties
| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| languageTags | Collection(Edm.String) | The list hosting a set of language tags for this resource. | 
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the resource, whether a topic is suggested, confirmed, or published. | 
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the resource. The data includes the user's feedback on the resource item. | 
| lastModifiedBy | microsoft.graph.identity | The last curator of the resource, if the resource has been curated | 
| lastModifiedDateTime | Edm.DateTimeOffset | The last curated time of the resource, if the resource has been modified | 

### Topic name
Topic name inherits from microsoft.graph.topicResourceBase, with an additional property named name, hosting the topic name string, as well as a list of properties in microsoft.graph.topicResourceBase describing how the name is associated with the topic.

#### Properties

| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| name | Edm.String | The property hosting the topic name string. | 
| languageTags | Collection(Edm.String) | The list hosting a set of language tags for this topic name. | 
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the name, whether a topic is suggested, confirmed, or published. | 
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the topic name. The data includes the user's feedback on the topic name. | 
| lastModifiedBy | microsoft.graph.identity | The last curator of the name, if the name has been curated | 
| lastModifiedDateTime | Edm.DateTimeOffset | The last curation time of the name, if the name has been curated | 

### Definition
Definition inherits from microsoft.graph.topicResourceBase, with an additional property named definition, hosting the topic definition string describing the topic, as well as a list of properties in microsoft.graph.topicResourceBase describing how the definition is associated with the topic.

#### Properties

| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| definition | Edm.String | The property hosting the definition string. |
| languageTags | Collection(Edm.String) | The list hosting a set of language tags for this definition. | 
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the definition, whether a topic is suggested, confirmed, or published. | 
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the definition. The data includes the user's feedback on the definition. | 
| lastModifiedBy | microsoft.graph.identity | The last curator of the definition, if the definition has been curated | 
| lastModifiedDateTime | Edm.DateTimeOffset | The last curation time of the definition, if the definition has been curated | 

### Site
Site inherits from microsoft.graph.topicResourceBase, it has an webUrl field hosting URL property to uniquely identify a site, it has an displayName hosting the display name of the site, as well as a list of properties in microsoft.graph.topicResourceBase describing how the site is associated with the topic.

#### Properties
| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| webUrl | Edm.String | The URL of site item. | 
| displayName | Edm.String | The display name of the site item. |
| languageTags | Collection(Edm.String) | The list hosting a set of language tags for this site. |
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the site, whether a site is suggested, confirmed, or published. |
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the site. The data includes the user's feedback on the site item. |
| lastModifiedBy | microsoft.graph.identity | The last curator of the site, if the site has been curated |
| lastModifiedDateTime | Edm.DateTimeOffset | The last curation time of the site, if the site has been curated |

### File
File inherits from microsoft.graph.topicResourceBase, it has an webUrl field hosting URL property to uniquely identify a file, it has an displayName hosting the display name of the file, as well as a list of properties in microsoft.graph.topicResourceBase describing how the file is associated with the topic.

#### Properties
| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| webUrl | Edm.String | The URL of file item. | 
| displayName | Edm.String | The display name of the file item. |
| languageTags | Collection(Edm.String) | The list hosting a set of language tags mined for this file. |
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the file, whether a file is suggested, confirmed, or published. |
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the file. The data includes the user's feedback on the file item. |
| lastModifiedBy | microsoft.graph.identity | The last curator of the file, if the file has been curated |
| lastModifiedDateTime | Edm.DateTimeOffset | The last curation time of the file, if the file has been curated |

### User
User inherits from microsoft.graph.topicResourceBase and microsoft.graph.identity, it has an id field to uniquely identify a person, it has an displayName hosting the display name of the user, it has an email hosting the email of the user, as well as a list of properties in microsoft.graph.topicResourceBase describing how the person is associated with the topic.

#### Properties

| Property       | Type           | Description                                 | 
| -------------- | -------------- | ------------------------------------------- | 
| id | Edm.String | The unique identifier of user id. | 
| email | Edm.String | The email address of user. | 
| displayName | Edm.String | The display name of the identity. |
| lifecycle | microsoft.graph.topicLifecycle | The lifecycle of the person, whether a person is suggested, confirmed, or published. |
| viewpoint | microsoft.graph.topicViewpoint | Represents user viewpoints data on the topic. The data includes the user's feedback on the topic item. |
| lastModifiedBy | microsoft.graph.identity | The last curator of the person, if the person has been curated |
| lastModifiedDateTime | Edm.DateTimeOffset | The last curation time of the person, if the person has been curated |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.qna",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.topic",
  "primaryName": "@odata.type": "microsoft.graph.topicName",
  "alternateNames": [
    { 
        "@odata.type": "microsoft.graph.topicName" 
    }
  ],
  "definition": {
    "@odata.type": "microsoft.graph.topicDefinition"
  },
  "lifecycle": {
    "@odata.type": "microsoft.graph.topicLifecycle"
  },
  "viewpoint": {
    "@odata.type": "microsoft.graph.topicViewpoint"
  },
  "webUrl": "String",
  "currentLanguagueTag": "String",
  "languageInfos":[
    {
    "@odata.type": "microsoft.graph.topicLanguageInfo"
    }
  ],
  "highlyRelatedFiles":[
    {
    "@odata.type": "microsoft.graph.topicFile"
    }
  ],
  "highlyRelatedSites":[
    {
    "@odata.type": "microsoft.graph.topicSite"
    }
  ],
  "highlyRelatedUsers":[
    {
    "@odata.type": "microsoft.graph.topicUser"
    }
  ],
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "lastModifiedDateTime": "Edm.DateTimeOffset"
}
```

