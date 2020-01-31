---
layout: post-no-feature
date: 2020-01-26 20:33:45
title: "Project: Updating Atlas"
categories: projects
author_name : binnur
author_url : /author/binnur
author_avatar: binnur
show_avatar : true
read_time : 3
feature_image: feature-birds
show_related_posts: false
square_related: recommend-plant
---
I am a [FIRST Robotics Competition](https://www.firstinspires.org/robotics/frc)
mentor with [Team 4915, Spartronics](http://spartronics4915.com). A couple of
weeks back, I took [Atlas](http://spartronics4915.com/about-2/our-robot/atlas/),
our first ever competition robot from 2014 home for some updates. As you can
see, she is pretty beaten up. Atlas is our trusty robot for community
demonstrations and July 4th parades.

![Atlas, 2014 Spartronics Robot]({{site.baseurl}}/img/assets/atlas.png)

This is not our first time updating Atlas. Two years ago, my hubby and I hosted
garage parties to fix her up. As she is our ever first robot, she is also very
dear to our heart.

She is the simplest robot we built to date: basic design, no fancy electronics
like encoders, no vision, ... Her autonomous code was basically *move forward
for x seconds, and shoot*. Yet, she hardly missed and even had a 50/50 chance
for receiving the bonus autonomous score. And, she took us to the FIRST World
Championship. Yes, we have a lot of great memories building her. Similarly, our
last upgrade was fun and engaging — I recall one of our students saying "Robot,
pizza, and dad jokes! What could be better!"

As it is the build season, I decided to take her home and give her an update.
My excuse, the 2020 WPI libraries are updated, and with that our old
command-base code is discontinued. I also wanted to integrate bling (LED
animations) to our robot for fun action.

It is interesting how a simple idea can have so many layers... As I went through
[the update
process](https://docs.wpilib.org/en/latest/docs/getting-started/getting-started-frc-control-system/offline-installation-preparations.html),
I noted all the different moving parts: roboRIO image update, firmware updates
for controllers, various pieces of driver station software, robot code itself...
And remember, she doesn't have any of the bells and whistles! It is such a
drastic difference from the low-code/no-code development platform trends.

>"There are only two hard things in Computer Science: cache invalidation and naming things."
>-- Phil Karlton

Updating and migrating the robot code had its moments… I am sure those commands
and methods made sense two years ago, but not now. Which was an opportunity to
further simplify the code, which should also help with future update cycles.

As I mentioned, one of my goals was to integrate LED system with our robot
actions, such as playing a fast-moving red LED animation when we are hunting for
a ball. After we synced up on the proof of concept design, hubby worked on the
Arduino side and I took on the robot code integration. 30 minutes later, we were
giggly when it all worked on first try -- nothing like blinking lights
to bring joy. :) It was even more fun to see mentor reactions when we
brought her back -- she is dear to our hearts!

I am already looking forward to her next update cycle!
