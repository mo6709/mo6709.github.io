---
layout: post
title:      "MVC The Long Short Way"
date:       2018-02-21 16:43:58 +0000
permalink:  mvc_the_long_short_way
---



The purpose of the web is to share and display data between computers, user can retrieve data and display it. After the user changes the date, the system stores the updates in the data center. Since the data flow between the user and data center, a developer may tempt to tie these two pieces together to make code more consolidate and improve performance. However this design process has significant problems. One is the user interface change more often than the data. Another problem with combining these two pieces together is that business logic is a way more complex than transmitting the data.

With that being said, how do you design a functional user interface so you can easily modify individual parts?

Model-View-Controller Pattern.
The MVC components and their interaction can make this process pleaser. Model is the biggest part of the application, it will keep the business logic separated while the view can be managed separately, instead of repeating code, the view can store templates and change only the parts that needs to be change. Controller will maneuver between the user requests to the logic and will tall view how to display the data accordingly.

Restaurant. Chef. Waiter.

Well this is something we all use to already, when you go to restaurant you seat on the table and the waiter serve you but you will never need to interact with the chef. The chef has all the recipes and knows the right amount of each ingredients in order to make the dish, then the waiter come to take the dish and serve it to you. With this analogy we can remind ourselves what are the responsibilities and to whom they belongs to. Model is the chef that knows how to prepare the data accordingly, then we have the controller which is the waiter that take requests from the user to the chef and then for the final step the controller ask the view to represent the data to the user.

Where did it start ?

Trygve Reenskaug introduced the MVC pattern in Smalltalk-76 while visiting the Xerox Palo Alto Research Center in 1970s. In the 1980s, Jim Althoff and other improved the MVC version for the Smalltalk-80. Later on 1988 the concept was expressed as a general concept. The popularity of MVC started in web applications after Apple introduced it in their WebObjects 1996, which was written in Objective-C and help enforce MVC principles. MVC web framework now is quite big relative to non-MVC web applications.


The Goals.
Simultaneous development is efficient when big teams working on one big application. MVC decouples the various components of application, developers are able to work in parallel on different parts without impacting one another. For example the front-end team can work on representing the data without having the dada ready and the back-end team can work on their tasks without having the front-end ready. Code reuse is available when creating components independently of one another, developer can reuse the components in different application easily.

Separation of Concerns.
Application design is a part of development, when you start to draw your application you will need to separate the responsibilities and make sure each component does one thing, but nothing other than that. The importance of separating the concerns is to make the code more manageable and understandable, where one component has its own mechanism it’s easy to maintain and hard to break especially in case of future development . Problems become more obvious and you can go direct to them without getting confused. Other developers would highly appreciate it where they know what is the purpose of each component.

Where to Find MVC?
Most of the application nowadays are based on MVC principale you most likely to find MVC in web application but it is very popular that you can find it in mobile application and desktop application as well. MVC was adapted by Java, C#, Objective-C, PHP, Ruby, Python and more. MVC’s popularity outside the traditional enterprise environmental which has long been popular.

Advantages & Disadvantages.

Simultaneous development allow multiple developers to work on the model, view and controller.
High cohesion, with MVC you can group logical action in same controller also the views for a specific model are group together.
The low coupling among models, views and controllers give a huge flexibility.
Modification and adding feature is ease because the separation of concerns, one model can have multiple views.
With all these advantages disadvantages come as well.

Code navigability can be very complex, hence it layers of obstruction and require the developer to adapt its decomposition criteria to MVC.
Multi-artifact will decompose a feature into three artifacts causes confusion. Thus, requiring developers to maintain consistency of multiple representation at once.
Knowledge of multiple technologies become the norm and MVC developers need to be skilled in multiple technologies.
