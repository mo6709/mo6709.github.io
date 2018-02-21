---
layout: post
title:      "JWT Token Authentication With React"
date:       2018-02-21 16:42:58 +0000
permalink:  jwt_token_authentication_with_react
---


The way to authenticate a user should be more pleasant for both sides, by saving a token on the client side we can easily let the user access thie data and make sure the communication secure enough.

Whaen creating  API backend for with authenticated data, it is importent to know how to make the proccess sooth as posiable in order to make the client side enjoing fast and secure flow. With the jwt token you can siplfy the proccess. it lets generate the token at backend with diffrent type of cryptograohy machanisem and attache to it a secret variable, then return the cryptic strings to the user. 

The client side save the sting on local machin the for every authenticaticated request it would sed it along with the request. the backend would take the cryptic string and would decrypte it to the required data.
