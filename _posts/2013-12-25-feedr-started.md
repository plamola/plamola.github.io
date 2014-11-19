---
layout: post
title: FeedR started
---
I decide to start writing my own RSS reader. 

Just because I can. 
Or at least it is something I should be able to do.

Ever since the announcement of the pending shutdown of Google Reader, I've been looking for an alternative. While hosted solutions like Newsblur & Feedly are sufficient for most users, I choose not to use them. Simply because it would introduce another dependency on the services of another company/individual. One day, the service will no longer be available.

Thats why I have chosen to host my own RSS reader, on a server which I maintain. I started using [TinyTinyRSS](http://tt-rss.org/redmine/projects/tt-rss) and it is working just fine. It also has a decent Android client, to replace Newsrob. To bad it doesn't have an offline mode.


Why build my own?
-------------
Two reasons.

First, I would like to use a RSS reader based on a language I know (or would like to get to know). This gives me the possibility to maintain and enhance the application, long after the original authors(s) have moved on to another project. Although TinyTinyRSS is open source, it is written in PHP. I have done some development work with PHP, but it is not something I particularly enjoyed. From a professional perspective, there isn't a lot of money the be made with having PHP skills.
This brings me to reason number two.

The second reason for writing my own RSS reader, is learning new skills. I'm a Java developer, but not one with in-depth knowledge of the lastest and greatest frameworks. Time to fix that.

Weapons of choice
-------------
I already have a list of frameworks/technologies I would like to use. 

1. Play 2 framework
  A long time ago I could infected by the Ruby on Rails (RoR) framework. I used it a couple of years and then forgot about it. Until I read about a major security problem, forcing me to upgrade my existing RoR applications. During the upgrade I got once again stuck in a Gem installation problem and suddenly remembered why I stopped using Ruby. Luckily I just heard about the Play framework. The ease of development reminded me of RoR, but I was using Java. I EOL'd all but one of my RoR applications and rewrote the remaining one using the Play framework. Since then, I've started development of another application [sendR](https://github.com/plamola/sendR), also using the Play Framework. Makes sense to use it again.

2. Scala
  With the Play framework, you can choose to use the Java or the Scala flavor. Even after choosing one, you can still use the other language too. To make it a challenge, I will use Scala for this application, knowing I could still fall back to Java, if needed.
  
3. Akka 
For retrieving the contents of the RSS feeds, I intent to use Akka. I've already used Akka in the [sendR](https://github.com/plamola/sendR) application and was impressed who easy it is to implement. The fact that is is included in the Play framework certainly helps.

4. Bootstrap 3
  In [sendR](https://github.com/plamola/sendR) I used bootstrap version 2.3. Time to upgrade my knowledge to the latest version.
  
5. AngularJS
  I've used Angular also in [sendR](https://github.com/plamola/sendR), so I might use it again.

6. Docker
	For shipping/installation I'm interested in using Docker. That is probably another project in itself. But its worth mentioning.

What's next
--------
I've created a [FeedR](https://github.com/plamola/FeedR) project on Github and made the first commits. First task is to get Akka up and running, retrieving the feeds.
