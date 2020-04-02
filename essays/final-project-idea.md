---
layout: essay
type: essay
title: "Final Project Idea: IDEA"
date: 2019-11-05
labels:
  - Software Engineering
  - Meteor
---

## Overview

<strong>Problem:</strong> Most students are generally shy and have a hard time introducing themselves to new people unless it's someone they sit next to in class. It's especially hard right now to meet new people, due to Covid-19.
  
<strong>Solution:</strong> My final project will be a mobile application that connects students through messaging.  The app will pair two users together each day with someone they haven't talked to yet.  Each morning they will get a message that says, "Hi (their name here), you have been paired with (their pairs name here) today. Say hi!" 

## Approach
Meteor is perfect for a messaging app given it's live updated local databases.  

  ### Mock up pages:
  <ul>
  <li>Landing Page with login and signup</li>
  <li>MyProfile (only the account owner can see)</li>
  <li>Profile (viewed by others)</li>
  <li>Terms of service</li>
  </ul>

## Use case ideas
<ul>
  <li>New user visits website, starts on landing page, creates an account, brought to profile page, informed a new match will be provided at 8am everyday.</li>
  <li>At 8am Monday the user gets a notification that he is paired with (another user) for that day. His match sends him a new message at 8:15am which says, "Hey there, want to go see a movie later? Jk we are doomed, Covid 19 is armageddon. Anyways, having a good day so far? I'm Rachel btw."</li>
  <li>At 8am Tuesday the user gets a new notification that he is paired with a new user for that day. He looks in his previous messages and finds that he can still message Rachel as well.</li>
  <li>The user realizes his new match, Frank, is a bit strange and doesn't want to talk anymore.  The user blocks Frank</li>
</ul>

## Beyond the basics
Eventually the app backend will include machine learning to optimize matches for compatability.  This will be a function of time spent talking to new matches.  The more time spent talking to new matches means the model fitness is improving.
