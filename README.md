# Application Programming Interfaces
## 1. APIs and Their Uses
An API, or Application Programming Interface, is set of functions, routines and tools for the use of building applications, which define the communications between another app, delivering and requesting from one another. There are numerous APIs that can help provide a programmer with the fundamentals to help develop an application. Though it varies on the definition of one, the common description of an API is that it can aid in developing programs but also provide communication between one another[1].
APIs are needed to help with data access and the mechanics to help make the software function. Retrieving data is key and APIs allow for this to be done as fast as possible, creating a front door to the data and can also create useable functions.

#### 1.1 Use of an API
There are different APIs that can be used for various reasons, for commercial and business use other than just for a developer. Twitter APIs allows for developers to gain access to the core twitter data and to allow access to search data and trend data to interact with. YouTube API allows for the integration of YouTube videos onto websites, rather than just linking the video and can also allow for data analysis on the videos.

## 2. Relationship with SDKs
An SDK, or Software Development Kit is a kit used for creating a program, providing the user a set of tools, libraries, code samples and guides in order for developers to create the application, be it either for software framework, computers, operating systems or video game consoles[2].

The difference between that of APIs and SDKs is that the latter are used for the creation of applications regardless of system and purpose while APIs are only used for specific purposes but with one main purpose; communicating with other applications.
However, SDKs do include an API for the whole reason of communications between applications, so it is fairly reliant on the APIs use, using them for the functions of the application. For instance, the Java Development kit, along with the compilers and other tools, has an API which is the libraries that make up its core programming language, for the developers to use within the SDK.

## 3. Incorporating an API
One such game that hit the market recently was ‘Assetto Corsa Competizione’, a racing simulator that aims to replicate the real world feeling of motorsports, by letting players be able to drive real cars with their exact specifications and are able to tune their cars to help with what race they are doing. The game includes real life race tracks and includes different racing divisions based on the type of cars used, along with many other features to accurately mimic actual motorsports. At the moment, the game is in early access, so it seems that it can be open to many ideas[3].

Most competitive games implement an API in terms of analysing stats and play sessions of the player, and in turn use that data to help out in matchmaking and leagues. In the eSports leagues, this is used heavily and can determine the best players from a league, making for a very competitive environment[4].

The idea is to have an API in Assetto Corsa Competizione that incorporates the same features that most competitive games have; to track the players’ stats. The main element of Assetto Corsa Competizione is that the sim racing aesthetic will come onto the multiplayer side of the game, so it would be beneficial to have an API that retrieves a player’s stats for use in terms of matchmaking and leagues.

Another use of the API being incorporated into the game would be use its prequel’s (Assetto Corsa) modding capabilities. That game allowed for players to create tracks based on the data from google maps or similar to help with creations of even more race tracks. It worked by receiving that data; getting elements such as land height and location data to turn the land into a playable area. This in turn would help expand the amount of content from the community and add to playability.

## 4. APIs with a range of uses
Many APIs are used for a variety of purposes, be it to retrieve specific types of data or to communicate with other applications to access different features. The Steam Web API is a web based API used to access Steamworks features, which these features are things like the stats and achievements and interacting with other steam users[5].

The API can be used by other web services but mostly by steam itself for any feature that is included in the steam store, anything from the store of steam games, the library of games that the player owns, the community hub and even the player’s activity. This is the general features that the player has access to when utilising steam and all receives data in relation to that feature. Steam Web API can also access data in regards to multiplayer games and achievements that can be used for comparison as well as just return the data of global players[6].

Other Websites can use the Steam Web API for use on their own services. Community gaming trading websites have come up ever since Valve implemented an item feature in Team Fortress 2 that allows for users to craft and trade their items and as such, these websites can display trade advertisements and receiving the data based on that item, located in their steam inventory. There are sites similar that offer similar services using the Steam Web API, such as weapon skins from other games that utilise the same item based features.

## 5. Application that utilises an API
### 5.1 Implementing an API
I will be using my game project to implement the API in. The project in question is called ‘Road Rage’, a racing game, but now, it is in the first prototype stage. The game will be developed in the latest version of Unity, the software that will be supporting the prototype. The idea is to create the program by using the tools given to develop the fundamental aspects of the game, to show off the features and create a general feel for how the game will function, implementing in features like the racetrack and placeholder cars.

The API I am planning to use is the Unity Scripting API, that comes with Unity to create the scripts for all the features in the prototype, including handling car structure and the controller manager. The main API I intend to use for the prototype is ‘UnityEngine’, giving me all the features available to help develop the scripts.

Details about the API can be found [here:](https://docs.unity3d.com/ScriptReference/index.html)[7]

### 5.2 Designing the application with the API
As stated before Unity incorporates a scripting API into its game engine, which is so that the user can use the libraries that Unity has in stock. This way the user can use additional tools than the elements that they already have, making development easier and simpler to develop.

These tools that Unity has can be incorporated into any genre of game, be it for a first-person shooter or a platformer. Unity even gives pre-built assets compromising of base structures, so the user can utilise them quicker and can learn about them during development. This will help me with the prototype that I am developing now, as I plan to utilise a base car rig, which the other cars will be based off. The values will be predefined in classes that will separate the make and model of the car, making each one unique.
The tools that I will be using within the prototype will be called the ‘BoxCollider’ and ‘WheelCollider’ tools. The ‘BoxCollider’ tool creates basic, primitive collision boxes that can be assigned to a game object or likewise. The idea here is to use this for creating the structure and body for the cars[8].

![Box](https://docs.unity3d.com/500/Documentation/uploads/Main/BoxCollider2.png)
[9]

The ‘WheelCollider’ is a special type of collider, where it is used for vehicle wheels and has numerous features, including a suspension model, motor power and brake settings. What is mainly important about the ‘WheelCollider’ is that it has its own physics model, separate from the usual one in Unity, that aims for more realistic behaviour and can have its own properties based on the road surface. Here, I intend to use this for the wheels of the car and which the features that API gives me can be used to create a handling model akin to the nature of the game[10].

![Wheel](https://vehiclephysics.com/img/components/vpp-wheelcollider.png)
[11]

The API in unity has a class in its library consisting of both these colliders to make up the cars in the prototype, which will help make up the positioning and values of the suspension, horsepower, etc. Not only will the scripting API be used for the cars but also the other elements such as the controller input and the camera controller, with their own predefined values and features that will help with the development of the game.

### 5.3 Developing the app with the API
The game was developed with the handling and the creation of the car done mainly with the scripting API.

![Demo](https://github.com/LBruni98/Road-Rage/blob/master/Development/Game%20Demo.PNG)

Below is the code taken from one of the scripts of the game, the car controller script.

```csharp
//This code utilises the UnityEngine API, which contains the features used to create this script and other scripts
using System.Collections;
using System.Collections.Generic;
using UnityEngine; //The API library in question

public class CarController : MonoBehaviour {

	public void GetInput() {
        m_horizontalInput = Input.GetAxis("Horizontal"); //Gets the horizontal controller inputs from the controller script, this being the left analogue stick
        m_verticalInput = Input.GetAxis("BothTriggers"); //Assigns the vertical input to both the Right and Left controller triggers
    }

    public void Steer()
    {
        m_steeringAngle = maxSteerAngle * m_horizontalInput; //For having the maximum amount of steering apply to the sticks
        wheelFL.steerAngle = m_steeringAngle; //This makes the front left wheel the wheel that turns
        wheelFR.steerAngle = m_steeringAngle; //This makes the front right wheel the wheel that turns
    }

    public void Accelerate() //FWD
    {
        wheelFL.motorTorque = m_verticalInput * motorPower; //For having the maximum amount of power apply to the pressure of the triggers. Assigns it to the front left
        wheelFR.motorTorque = m_verticalInput * motorPower; //For having the maximum amount of power apply to the pressure of the triggers. Assigns it to the front right
    }

    //This piece of code updates the rotation of the wheels and applys the animation to each wheel
    private void UpdateWheelPosition()
    {
        UpdateWheelPose(wheelFL, transformFL);
        UpdateWheelPose(wheelFR, transformFR);
        UpdateWheelPose(wheelRL, transformRL);
        UpdateWheelPose(wheelRR, transformRR);
    }
    
    //Making the wheels turn
    private void UpdateWheelPose(WheelCollider collider, Transform transform)
    {
        Vector3 pos = transform.position; //Gets the position of each wheel
        Quaternion quat = transform.rotation; //Provides rotation to the wheels

        collider.GetWorldPose(out pos, out quat); //Gets the world position of the wheels

        transform.position = pos;
        transform.rotation = quat;
    }

    private void FixedUpdate()
    {
        GetInput(); //Gets the input of the player
        Steer(); //Steering class
        Accelerate(); //Makes the car move
        UpdateWheelPosition(); //Wheels rotation

        rb = this.GetComponent<Rigidbody>(); //Applys it to the rigidbody component (the car)
        AnalogueSpeed.ShowSpeed(rb.velocity.magnitude,0,100); //Displays the speed of the car as a speedometer.
    }

  private float m_horizontalInput;
  private float m_verticalInput;
  private float m_steeringAngle;
  
  public WheelCollider wheelFL, wheelFR;
  public WheelCollider wheelRL, wheelRR;
  public Transform transformFL, transformFR;
  public Transform transformRL, transformRR;
  public float maxSteerAngle = 30;
  public float motorPower = 300;
  public Rigidbody rb;
}
```
The key points of the script are the ‘WheelCollider’ variables, these being unique to unity and helped with the development of the wheel position, rotation and power and steering of the car. Quaternion is a feature from the API that is used to represent rotations and are applied to the wheels of the car to determine the rotations.

Another point is the input. In conjunction with the input manager, this is used to help code the inputs and can receive the inputs from the player. This was used to determine the amount of power and brake force based on the car was going to be applied to the acceleration and braking.

Below are the wheel colliders applied to the car.

![Wheels in Action](https://github.com/LBruni98/Road-Rage/blob/master/Development/WheelColliders.PNG)

### 5.4 Testing
#### 5.4.1 White Box

#### 5.4.2 Black Box

#### 5.4.3 Improvements

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

ATTACKS RELATING TO APIS (DONE)

CASE STUDIES ()

CONCLUSION ()
```
#### References
1. Vangie Beal (2000). API - application program interface. [online]. Webopedia. Available from: <https://www.webopedia.com/TERM/A/API.html>. [Accessed 6 November 2018].
2. Margaret Rouse (2005). software developer's kit (SDK). [online]. WhatIs.com. Available from: <https://whatis.techtarget.com/definition/software-developers-kit-SDK>. [Accessed 6 November 2018].
3. Assetto Corsa Competizione [online]. (2018). Available from: <https://www.assettocorsa.net/competizione/>. [Accessed 16 December 2018].
4. Abios [online]. (2018). Available from: <https://abiosgaming.com/esports-data/api/>. [Accessed 16 December 2018].
5. SteamWorks [online]. (n.d). Available from: <https://partner.steamgames.com/doc/webapi_overview>. [Accessed 4 December 2018].
6. Steam Web API [online]. (2010). Available from: <https://developer.valvesoftware.com/wiki/Steam_Web_API>. [Accessed 4 December 2018].
7. Unity Documentation [online]. (2018). Available from: <https://docs.unity3d.com/ScriptReference/index.html>. [Accessed 16 December 2018].
8. Unity Documentation [online]. (2014). Available from: <https://docs.unity3d.com/ScriptReference/BoxCollider.html>. [Accessed 16 December 2018].
9. Unity (n.d). A real-world Compound Collider setup [online]. Available from: <https://docs.unity3d.com/500/Documentation/Manual/class-BoxCollider.html>. [Accessed 16 December 2018].
10. Unity Documentation [online]. (2014). Available from: <https://docs.unity3d.com/ScriptReference/WheelCollider.html>. [Accessed 16 December 2018].
11. Vehicle Physics Pro (2015). VP WheelCollider [online]. Available from: <https://vehiclephysics.com/components/wheel-collider/>. [Accessed 16 December 2018].
