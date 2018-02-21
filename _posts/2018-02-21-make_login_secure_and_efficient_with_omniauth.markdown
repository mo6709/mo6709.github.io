---
layout: post
title:      "Make Login Secure and Efficient With Omniauth"
date:       2018-02-21 17:09:29 +0000
permalink:  make_login_secure_and_efficient_with_omniauth
---


Why ask your user for credentials and maintain them with high risk with hard work around the clock while you can provide your client with top security in matter of minutes.

In this post we will walk through the process of implement the amazing gem omniauth. 

lets first describ the problem.
The one think, you most remember all of the password, perhaps you have password maneger which comes with its on complexety. A big persentage would forget the password over the time. The big issue with password once you ask user to sighn up with password the would live the and would never come back.

And here is the biges problem once Rails store the password securlly on the database they stored secured but what if someone gain access to the server, they instruct the server to serve them with all the sensetive credentials. Then you would need to maintan emails passwords recavery, a lots of pain! 

Lets explain an Omniauth strategy.
Once the user get to your site the asked to be logged in. Then they would be redirected to login screen.
The login screen sugests to options of an account with Google or Facebook. The user clicks the button to login with Google which send the user to the site/auth/google and redirect them to Google signin page. If the user is not loogedin to Google they reqiure to log in manualy, most likly they are loggedin to their account. once the loggedin to their Google account the ask to graind promition to your site to access the user's information. 
The user will be redirected back to your site/auth/google/callback, then from there to the page initialy requested.


Use Omniauthto to handle authentication in Rails server.


