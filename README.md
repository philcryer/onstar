On-Star

On-Star
======
*is it good, or is it whack?* 

![OnStar logo, ftw!](https://upload.wikimedia.org/wikipedia/en/2/29/On_star1234-.jpg)

This is a study looking at the specifics of On-Star (and competing products) data gathering, transmission and storing procedures. What do they collect; how do they handle/protect the data they save; what *can* they do with user data? After this, we'll have a feasibility study to see if we want to make a talk out of this for infosec/privacy cons. 

Genisis of this question
=======
Last week I at Infowarcon (http://infowarcon.com/) in Nashville I floated my idea of investigating the auto insurance boxes that you install that give you lower rates if you allow them to monitor you. People liked that, but then we got into On-Star and trying to understand what they collect, how they transmit it, how they store your data and what they can do with it later. This seemed to have a broader interest because it's not voluntary like the auto insurance box, plus it's more standardized, with other car companies coming up with their own On-Star like solution, and their EULAs could be completely different.

What is On-Star?
===========
OnStar Corporation is a subsidiary of General Motors that provides subscription-based communications, in-vehicle security, hands free calling, turn-by-turn navigation, and remote diagnostics systems throughout the United States, Canada and China.

Linky:

* https://en.wikipedia.org/wiki/OnStar
* https://www.onstar.com/
* http://auto.howstuffworks.com/onstar2.htm

How does On-Star work?
=================

Summarize the great overview at [How stuff works](http://auto.howstuffworks.com/onstar2.htm)

OnStar Technology
===============
At its most basic, OnStar consists of four different types of technology: cellular, voice recognition, GPS and vehicle telemetry. All of the services that OnStar provides are a result of one or more of these technologies working together.

![OnStar advisor, who is very happy to take your call apparently!](http://static.ddmcdn.com/gif/onstar-3.jpg)

OnStar's cellular service is voice-activated and hands-free. The console contains a built-in microphone and uses the car speakers. To make a call, you speak a phone number or a previously stored name associated with a phone number. The console is connected to a Vehicle Comm and Interface Module (VCIM), which uses a cellular antenna on top of the car to transmit signals to OnStar's cellular network. (For more information on cellular technology, see How Cell Phones Work.) OnStar's cellular service has a better range than most cell phones (although you can still lose service in remote areas), with a full three watts instead of a regular cell phone's 0.6 watts. With some OnStar plans, you can also use the cellular service just as you would a regular cell phone plan.


For calls to the advisor, OnStar uses voice recognition software similar to that already used in some hand-held cell phones. However, one of OnStar's unique features is the ability to "surf the Web" using the Virtual Advisor automated system. For this service, OnStar uses text-to-voice technology called VoiceXML. When you ask for information, such as "weather," the software translates your request into XML (Extensible Markup Language) and matches it to settings in your OnStar profile. Then it translates the information into VoiceXML and reads it to you.

 
Photo courtesy OnStar Corporation 
An OnStar advisor
The GPS receiver is called OnCore, and it is part of the VCIM (older OnStar-equipped vehicles have separate modules for the cell phone and GPS system). A GPS receiver uses the amount of time that it takes for a radio signal to get from satellites to a specific location to calculate distance. (For more information on GPS, see How GPS Receivers Work). The OnStar Call Center uses four different satellites to pinpoint the car's location when either the driver or the car itself asks to be located.

![How it works, isn't that lady on the bottom pretty evil looking?](http://static.ddmcdn.com/gif/onstar-7.jpg)
 
To give a vehicle the ability to call when it is in an accident, OnStar uses an event data recorder (also known as a crash data recorder). GM calls the entire process the Advanced Automatic Crash Notification System (AACN). It's the car's equivalent of an airplane's black box, except that the AACN only starts recording in the event of a crash and only records data.

The AACN system comprises four components: sensors, the Sensing Diagnostic Module (which includes the event data recorder), the VCIM and the cellular antenna. The number and location of sensors vary depending on the specific car, but they all work the same way. When the car is in a crash, sensors transmit information to the Sensing Diagnostic Module (SDM). The SDM also includes an accelerometer, which measures the severity of the crash based on gravitational force. (The range is 1.0 to 2.0 gs, depending on the vehicle.)

  
![Advanced Automatic Crash Notification System](https://www.dropbox.com/s/qzk73wfghs2e94f/Screenshot%202014-01-26%2022.55.31.png) 

The SDM sends this information to the VCIM, which uses the cellular antenna to send a message to the OnStar Call Center. When an advisor receives the call, he uses the GPS to find the vehicle's location and calls the car to check with the driver. Even if there's not a measurable impact, the VCIM also sends a message when the air bag goes off, prompting the advisor to call the car's driver.

Next, we'll learn exactly what kind of services OnStar provides and see how to use them.


Event Data Recorders and OnStar Statistics
==
	Although OnStar is relatively new, event data recorders are not. GM first used a type of event data recorder (EDR) in the mid-1970s in conjunction with air bags, and the technology has continued to evolve. In the mid-1990s, GM began using them in racecars and some passenger vehicles to collect crash-related data. Today the National Transportation Safety Board (NTSB) estimates that 65 percent to 90 percent of vehicles in the United States contain some type of EDR. Often the driver doesn't even know that it's there [ref]. In 2004, the National Highway Traffic Saftey Administration recommended that EDRs installed in vehicles built after September 1, 2008 meet a set of minimum standards. The NTSB wants to go one step further and make standardized EDR installation mandatory for all manufacturers.
	In September 2005, OnStar handled, on average:

	383,000 calls
	43,000 remote unlocks
	900 air bag deployments
	420 stolen vehicle locations
	15,000 emergency calls
	23,000 roadside assistance calls
	9.5 million hands-free calls
	Source: OnStar Press Room 
