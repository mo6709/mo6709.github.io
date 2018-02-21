---
layout: post
title:      "Asynchronous Rails with Sidekiq"
date:       2018-02-21 17:57:46 +0000
permalink:  asynchronous_rails_with_sidekiq
---


Lets move the long runiung process to the background.
Once the user use a single thred system it can be efficent for the dev team but what about the actual user, they can get fustrated at our wonderful and efficent system that we built. 

One senerio is whiale a Sals team need to do long task on like uploding more records to the database thir task is really to get back to sale so when they need to get back to thir primey task we should not stop them. Uploding nig amount of data can take awhile why do we need to let the user babydite the system while uploading instead we promise the user that we will get back once everithing got uploaded or otherwise.

This were worker comes in, with long runing tasks that require no attantions we can move them to the backround and get back to it once they done.
Rails will open different branch and execute the long runing tasks as new thred. 
