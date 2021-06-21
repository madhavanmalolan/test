# io.swagger.client - Kotlin client library for Public APIs

## Requires

* Kotlin 1.4.30
* Gradle 5.3

## Build

First, create the gradle wrapper script:

```
gradle wrapper
```

Then, run:

```
./gradlew check assemble
```

This runs all tests and packages the library.

## Features/Implementation Notes

* Supports JSON inputs/outputs, File inputs, and Form inputs.
* Supports collection formats for query parameters: csv, tsv, ssv, pipes.
* Some Kotlin and Java types are fully qualified to avoid conflicts with types defined in Swagger definitions.
* Implementation of ApiClient is intended to reduce method counts, specifically to benefit Android targets.

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://staging.questbook-dev.net*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthenticationApi* | [**completeAuth**](docs/AuthenticationApi.md#completeauth) | **POST** /auth/complete/{flow}/{session_id} | Complete Authentication
*AuthenticationApi* | [**executeAuthAction**](docs/AuthenticationApi.md#executeauthaction) | **POST** /auth/action/{action}/{session_id} | Execute Auth Session Action
*AuthenticationApi* | [**getAuthToken**](docs/AuthenticationApi.md#getauthtoken) | **POST** /auth/token/{session_id} | Generate a Token
*AuthenticationApi* | [**initiateAuth**](docs/AuthenticationApi.md#initiateauth) | **POST** /auth/initiate/{flow} | Initiate Authentication
*NftLApi* | [**getNftlBackground**](docs/NftLApi.md#getnftlbackground) | **POST** /nftl/{subquest_id}/background | Get the Background Image for an NFT
*NftLApi* | [**sendNftlSigningRequest**](docs/NftLApi.md#sendnftlsigningrequest) | **POST** /nftl/request | Send Signing Request
*NftLApi* | [**signNftl**](docs/NftLApi.md#signnftl) | **POST** /nftl/{nftl_request_id}/sign | Sign or Reject NFT-L
*NotificationsApi* | [**getPendingNotifications**](docs/NotificationsApi.md#getpendingnotifications) | **GET** /notification/{quest_id} | Get Pending Notifications
*QuestManagementApi* | [**createQuest**](docs/QuestManagementApi.md#createquest) | **POST** /quest | Create Quest
*QuestManagementApi* | [**createSubquest**](docs/QuestManagementApi.md#createsubquest) | **POST** /quest/{quest_id}/subquest | Create a Subquest
*QuestManagementApi* | [**getParticipatedQuests**](docs/QuestManagementApi.md#getparticipatedquests) | **GET** /quest/participated | Get Quests (Participated or Created)
*QuestManagementApi* | [**getQuestChatParameters**](docs/QuestManagementApi.md#getquestchatparameters) | **POST** /quest/{quest_id}/chat | Get Chat Details for Quest
*QuestManagementApi* | [**getQuestFeed**](docs/QuestManagementApi.md#getquestfeed) | **GET** /quest/feed | Get All Quests
*QuestManagementApi* | [**getSubquests**](docs/QuestManagementApi.md#getsubquests) | **GET** /quest/{quest_id}/subquest | Get Subquests of a Quest
*UserManagementApi* | [**getProfile**](docs/UserManagementApi.md#getprofile) | **GET** /user | Get User Profile
*UserManagementApi* | [**updateProfile**](docs/UserManagementApi.md#updateprofile) | **PATCH** /user | Update User Profile

<a name="documentation-for-models"></a>
## Documentation for Models

 - [io.swagger.client.models.Body](docs/Body.md)
 - [io.swagger.client.models.Body1](docs/Body1.md)
 - [io.swagger.client.models.Body2](docs/Body2.md)
 - [io.swagger.client.models.Body3](docs/Body3.md)
 - [io.swagger.client.models.Body4](docs/Body4.md)
 - [io.swagger.client.models.Content](docs/Content.md)
 - [io.swagger.client.models.Error](docs/Error.md)
 - [io.swagger.client.models.ErrorMeta](docs/ErrorMeta.md)
 - [io.swagger.client.models.InlineResponse200](docs/InlineResponse200.md)
 - [io.swagger.client.models.InlineResponse2001](docs/InlineResponse2001.md)
 - [io.swagger.client.models.InlineResponse2001Data](docs/InlineResponse2001Data.md)
 - [io.swagger.client.models.InlineResponse2001DataExpiry](docs/InlineResponse2001DataExpiry.md)
 - [io.swagger.client.models.InlineResponse2002](docs/InlineResponse2002.md)
 - [io.swagger.client.models.InlineResponse2003](docs/InlineResponse2003.md)
 - [io.swagger.client.models.InlineResponse2004](docs/InlineResponse2004.md)
 - [io.swagger.client.models.InlineResponse2005](docs/InlineResponse2005.md)
 - [io.swagger.client.models.InlineResponse2006](docs/InlineResponse2006.md)
 - [io.swagger.client.models.InlineResponse2007](docs/InlineResponse2007.md)
 - [io.swagger.client.models.InlineResponse2007Data](docs/InlineResponse2007Data.md)
 - [io.swagger.client.models.InlineResponse200Data](docs/InlineResponse200Data.md)
 - [io.swagger.client.models.InlineResponse201](docs/InlineResponse201.md)
 - [io.swagger.client.models.InlineResponse2011](docs/InlineResponse2011.md)
 - [io.swagger.client.models.InlineResponse2011Data](docs/InlineResponse2011Data.md)
 - [io.swagger.client.models.InlineResponse201Data](docs/InlineResponse201Data.md)
 - [io.swagger.client.models.InlineResponse400](docs/InlineResponse400.md)
 - [io.swagger.client.models.Links](docs/Links.md)
 - [io.swagger.client.models.Meta](docs/Meta.md)
 - [io.swagger.client.models.NFTL](docs/NFTL.md)
 - [io.swagger.client.models.OneOfbody1](docs/OneOfbody1.md)
 - [io.swagger.client.models.ParticipatedQuest](docs/ParticipatedQuest.md)
 - [io.swagger.client.models.Quest](docs/Quest.md)
 - [io.swagger.client.models.QuestAuthor](docs/QuestAuthor.md)
 - [io.swagger.client.models.QuestChat](docs/QuestChat.md)
 - [io.swagger.client.models.QuestChatChat](docs/QuestChatChat.md)
 - [io.swagger.client.models.QuestChatQuest](docs/QuestChatQuest.md)
 - [io.swagger.client.models.QuestChatSubquests](docs/QuestChatSubquests.md)
 - [io.swagger.client.models.QuestChatSubquestsCurrent](docs/QuestChatSubquestsCurrent.md)
 - [io.swagger.client.models.QuestCommonPayload](docs/QuestCommonPayload.md)
 - [io.swagger.client.models.QuestCommonPayloadDescription](docs/QuestCommonPayloadDescription.md)
 - [io.swagger.client.models.QuestRequirement](docs/QuestRequirement.md)
 - [io.swagger.client.models.QuestSubquests](docs/QuestSubquests.md)
 - [io.swagger.client.models.Subquest](docs/Subquest.md)
 - [io.swagger.client.models.UserProfile](docs/UserProfile.md)
 - [io.swagger.client.models.UserProfileWallets](docs/UserProfileWallets.md)

<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="JWT"></a>
### JWT


# test
