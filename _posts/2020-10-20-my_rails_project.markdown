---
layout: post
title:      "My Rails Project"
date:       2020-10-20 22:18:36 +0000
permalink:  my_rails_project
---


My rails project went smooth until halfway through my project, I started getting an error. I setup my project so a Host can make listings of their place that they want to rent out. When the user gets deleted, the listings that the user created was still on web app. Whenever the app tries the render the listing then it throws errors, not knowing who the listing belongs to. In my sinatra project i have to use @user.listings.destroy in the user#destroy controller. Rails has made it alot easier by using a simple macro. In the user model, i just need to add `:dependent` to the has_many listings. Rails then knows that when that user gets deleted then it will delete dependents with it.In this case the dependent is the listing. After inputting that code, my app starting running great again. Ruby on Rails is awesome!
