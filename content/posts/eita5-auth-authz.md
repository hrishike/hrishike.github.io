---
title: "Auth and Authz for a 5 yr old"
date: 2025-04-15T20:58:03+05:30
draft: false
publishdate: 2025-04-15
---

# Authentication and Authorization to a 5yr old


The purpose of this article is to help understand concepts by breaking them down and drawing parallels in the world to give the reader a model to understand them. Try to explain them as if you were explaining it to a 5 year old. 

Here is an attempt to explain Authorization and Authentication. 


Lets take a visit to a theme park as an example. You and your 5 year old visit a theme park say, Disney world or Universal studios. And there are lots of fun activities within the park such as fun rides, theme based activities etc.

:point_right: Authentication = Getting into the park (proving who you are)
:point_right: Authorisation = Which rides and areas you can access (what you’re allowed to do)

# Authentication
### Password-Based Authentication
This is like saying a code word at the Entrance
You arrive at the park, and the guard asks, “What’s the code word?”
You say, “Rollercoaster”, and they let you in.
This would be password based authentication. You know the passcode and they allow you to enter the park.
The problem is that if someone else hears the code word, they can get in too!

### Multi-Factor Authentication (MFA) 
Ticket + ID Check. The gate guard now asks for two things before letting you in: Your ticket and a proof of your Identity. This is to make sure it really is you.
Using this even if someone finds a ticket, they can’t enter without the identification being checked!


### Single Sign-On (SSO) 
One Wristband for all park rides. Instead of proving your identification and validating the ticket on every ride in the theme park. The theme park gives you a band which you put it on your wrist to identify that you can go on all rides. The wrist band can be bright in color and can be spotted from a long way away.
So, the check for your ID and ticket happens only at the entrance of the park and then your wrist band works as the identity proof.

### OAuth
Somebody with authority vouches for you.
Say you forget your ticket at home, but you know the manager of the theme park. The gatekeeper trusts the manager of the theme park and the manager trusts you. So, when the theme park manager says “Hey, I know them! I know they have bought tickets. Please let them in!”
The identity is proved through a mutually trusted party and hence the gatekeeper lets you enter without a ticket.


### Certificate-Based Authentication
Say you have won a golden pass which was issued by the theme park last saturday and this allows you to skip all the security checks. You carry this golden pass, just show this special pass and walk in.


### Token-Based Authentication 
Thumb imprint for all the rides
Here, the gatekeeper would take your thumb imprint when you get into the theme park, validate that and using that thumb imprint you can go on all the rides just showing the ink mark on your thumb when you entered. The ink will stay for 8 hrs only so make sure you sit on all the rides before that.


# Authorization
Now, just because you’re inside the amusement park does not mean you can go on every ride.

### Role-Based Access Control (RBAC) 
The easiest way is to permit going on rides based on say coloured wristbands in the park. In this case the park would give out different coloured wristbands based on the ticket that we purchase:

* Regular Pass  → Access to all basic rides.
* VIP Pass → Access to all rides, including roller coaster rides.
* Staff Pass → Allowed in restricted areas as well as all the above rides.
* Manager Pass → Can enter everywhere

### Attribute-Based Access Control (ABAC)

You get permitted to ride a rollercoaster with a check such as say height has to be above X cm & age should be above Y yrs.
So, access to certain things are based on the characteristics or attributes that you carry. 

In this case the park would have rules such as:
* 	Only people taller than 120 cm can ride the roller coaster.
* 	Only kids under 5 can enter the soft play area.
* 	Food is free for people who hold the VIP pass.