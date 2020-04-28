# VRChat API Documentation

!> **Super Important!** Using this API is allowed for non malicious usage. Abuse of the API may result in account termination!

?> These docs are for SDK version `2018.05.04.09.53` and build tag `build-18-05-18-noah-salmon`

# Documentation Information

Sections of the documentation which are labeled **Outdated** means the the article or endpoint is no longer supported be the current API version or we are still working on making sure the endpoint is still working.

Sections labeled **Soon** are work in progress articles and will be added to the documentation on future updates.

Sections labeled **BETA** are API endpoints found in the beta client of VRChat, and are subject to change as the features are finalized.

# API Libraries

1. ~~VRChatJava (Java) https://github.com/VRChatAPI/VRChatJava~~ outdated

2. VRChat.Net (C#) https://github.com/VRChatAPI/VRChat.Net


# Links to APIs

Right now there are 3 different options

1. Dev API - https://dev-api.vrchat.cloud/api/1/ (Not Documented)
2. Beta API - https://beta-api.vrchat.cloud/api/1/ (Not Documented)
3. Release API - https://api.vrchat.cloud/api/1/

In the docs we just use the Release but you can manually change it if needed

# Quick overview

VRChat uses the HTTP procotol to get basic information from the server and send information to the server.

## Authentication

Most of the APIs require you to be authenticated.

There are two ways to authenticate (technically one)

1. Send the Authorization header with Basic authentication
2. After calling the any API with Basic authentication save and reuse the returned `auth` cookie.

The second option is probably more recommended

## Client API Key

Every API requires you to give a special API key. To get it simply call the [Remote Config](RemoteConfig.md) endpoint.

The API key is passed in a query string named `apiKey`

?> Last Known key is `JlE5Jldo5Jibnk5O5hTx6XVqsJu4WJ26`
