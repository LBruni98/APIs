# Application Programming Interfaces
## APIs and Their Uses
An API, or Application Programming Interface, is set of functions, routines and tools for the use of building applications, which define the communications between another app, delivering and requesting from one another. There are numerous APIs that can help provide a programmer with the fundamentals to help develop an application. Though it varies on the definition of one, the common description of an API is that it can aid in developing programs but also provide communication between one another[1].
APIs are needed to help with data access and the mechanics to help make the software function. Retrieving data is key and APIs allow for this to be done as fast as possible, creating a front door to the data and can also create useable functions.

### Use of an API
There are different APIs that can be used for various reasons, for commercial and business use other than just for a developer. Twitter APIs allows for developers to gain access to the core twitter data and to allow access to search data and trend data to interact with. YouTube API allows for the integration of YouTube videos onto websites, rather than just linking the video and can also allow for data analysis on the videos.

## Relationship with SDKs
An SDK, or Software Development Kit is a kit used for creating a program, providing the user a set of tools, libraries, code samples and guides in order for developers to create the application, be it either for software framework, computers, operating systems or video game consoles[2].

The difference between that of APIs and SDKs is that the latter are used for the creation of applications regardless of system and purpose while APIs are only used for specific purposes but with one main purpose; communicating with other applications.
However, SDKs do include an API for the whole reason of communications between applications, so it is fairly reliant on the APIs use, using them for the functions of the application. For instance, the Java Development kit, along with the compilers and other tools, has an API which is the libraries that make up its core programming language, for the developers to use within the SDK.

## Incorporating an API
One such game that hit the market recently was ‘Assetto Corsa Competizione’, a racing simulator that aims to replicate the real world feeling of motorsports, by letting players be able to drive real cars with their exact specifications and are able to tune their cars to help with what race they are doing. The game includes real life race tracks and includes different racing divisions based on the type of cars used, along with many other features to accurately mimic actual motorsports. At the moment, the game is in early access, so it seems that it can be open to many ideas.

Most competitive games implement an API in terms of analysing stats and play sessions of the player, and in turn use that data to help out in matchmaking and leagues. In the eSports leagues, this is used heavily and can determine the best players from a league, making for a very competitive environment.

The idea is to have an API in Assetto Corsa Competizione that incorporates the same features that most competitive games have; to track the players’ stats. The main element of Assetto Corsa Competizione is that the sim racing aesthetic will come onto the multiplayer side of the game, so it would be beneficial to have an API that retrieves a player’s stats for use in terms of matchmaking and leagues.

Another use of the API being incorporated into the game would be use its prequel’s (Assetto Corsa) modding capabilities. That game allowed for players to create tracks based on the data from google maps or similar to help with creations of even more race tracks. It worked by receiving that data; getting elements such as land height and location data to turn the land into a playable area. This in turn would help expand the amount of content from the community and add to playability.

## APIs with a range of uses
Many APIs are used for a variety of purposes, be it to retrieve specific types of data or to communicate with other applications to access different features. The Steam Web API is a web based API used to access Steamworks features, which these features are things like the stats and achievements and interacting with other steam users[3].

The API can be used by other web services but mostly by steam itself for any feature that is included in the steam store, anything from the store of steam games, the library of games that the player owns, the community hub and even the player’s activity. This is the general features that the player has access to when utilising steam and all receives data in relation to that feature. Steam Web API can also access data in regards to multiplayer games and achievements that can be used for comparison as well as just return the data of global players[4].

Other Websites can use the Steam Web API for use on their own services. Community gaming trading websites have come up ever since Valve implemented an item feature in Team Fortress 2 that allows for users to craft and trade their items and as such, these websites can display trade advertisements and receiving the data based on that item, located in their steam inventory. There are sites similar that offer similar services using the Steam Web API, such as weapon skins from other games that utilise the same item based features.

## Security Issues surrounding APIs
Being that APIs are used primarily for data based services, it would pose as a great risk should the data being taken be used for malicious intent. This section of APIs will evaluate the security exploits and potential attacks that surround that of APIs.

### API based Attacks
#### Parameter Attacks
This submits unexpected data to take advantage of weaknesses in a database or program, SQL attacks being a prime variant of parameter attack. How this ties into APIs is that it states the parameter’s primary usage via name, making the attacker’s job easier.

#### Identity attacks
In order to help an API recognize an app, they need a code of some sort. This is known as an API key and apart from identifying the app, these have to be secret and hidden by the developers. The problem arises that it is fairly easy to uncover them and in turn can be used by attackers, commonly, by creating an accurate representation of a legitimate app to take users’ credentials for their own gain.

#### Man in the Middle
Within an interaction between a user/app and an API, it is possible for an attack to stand between them, intercepting the traffic and interfering with the conversation. These attacks, so called Man in the Middle, have an attacker intercept to have the interaction happen with them, rather than the API, at which here they can receive anything important to the user such as personal or bank account information. An attack like this is possible because of the lack of an API making use of the SSL/TLS layer properly, if not at all.

```
GENERAL INTRODUCTION (DONE)

SECTION(S) ON HOW THE API AFFECT SECURITY/A PROGRAM ()

ATTACKS RELATING TO APIS ()

CASE STUDIES ()

CONCLUSION ()
```
#### References
1. Vangie Beal (2000). API - application program interface. [online]. Webopedia. Available from: <https://www.webopedia.com/TERM/A/API.html>. [Accessed 6 November 2018].
2. Margaret Rouse (2005). software developer's kit (SDK). [online]. WhatIs.com. Available from: <https://whatis.techtarget.com/definition/software-developers-kit-SDK>. [Accessed 6 November 2018].
3. SteamWorks [online]. (n.d). Available from: <https://partner.steamgames.com/doc/webapi_overview>. [Accessed 4 December 2018].
4. Steam Web API [online]. (2010). Available from: <https://developer.valvesoftware.com/wiki/Steam_Web_API>. [Accessed 4 December 2018].
