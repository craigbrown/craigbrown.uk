---
layout: post
title: OrderEats - a new platform for ordering food
date: 2017-10-12 13:36:20 +0100
#description:
img: OrderEatsLogo.jpg
tags: [Projects, Android]
---
For my summer project at UCL, I chose to create a food ordering application for Android which was backed by an API written in Go, using a MySQL database. You're probably already wondering, "why do we need another food ordering service?" - after all, we already have Deliveroo, UberEats, JustEat, etc, etc. But I think there is a gap for a new type of service.

<p style="text-align: center;">
![OrderEats Restaurant Selection Screen]({{site.baseurl}}/assets/img/OrderEatsScreen4.png)<br>
**_The OrderEats order receiving tablet app for restaurants._**
</p>

## The state of the industry

The existing food ordering apps can be boiled down to three types.

Firstly, there are the aggregators like JustEat. They sign up existing takeaway restaurants which already have their own delivery operations, and connect them to their customers via an app. Their main product is the software, and they don't get involved in the actual delivery operations.

Secondly there are the newer delivery services like Deliveroo. They do provide the software, but they also provide the delivery operations. This opens up these services to restaurants which don't or can't hire their own delivery drivers, but the downside is a hefty commission fee of up to 30%. As a result, prices on these apps are sometimes inflated compared to the price in the restaurant.

Finally there are the order-ahead apps provided by companies like McDonald's and Starbucks. They don't allow delivery at all, so are only aimed at improving the experience of customers who come in to pick up food (or coffee). These are becoming popular with large chains, but smaller businesses just don't have the resources to create their own order-ahead apps.

There's no solution for small businesses that want an order-ahead app but can't afford to make their own, and don't want the added cost of providing delivery. That's where OrderEats comes in.

## A new platform

<p style="text-align: center;">
![OrderEats Restaurant Selection Screen]({{site.baseurl}}/assets/img/OrderEatsScreen1.png){:height="30%" width="30%"}
![OrderEats Menu Screen]({{site.baseurl}}/assets/img/OrderEatsScreen2.png){:height="30%" width="30%"}
![OrderEats Order Screen]({{site.baseurl}}/assets/img/OrderEatsScreen3.png){:height="30%" width="30%"}<br>
**_The OrderEats smartphone app for customers. These images show the flow for a customer placing an order. The designs make heavy use of the Material Design framework, ensuring a familar and consistent user experience._**
</p>

OrderEats consists of two Android applications written in Java. One is a smartphone app that allows the customer to choose a nearby restaurant, browse their menu, and place an order. The other is a tablet app, provided to the restaurant to allow them to view incoming orders and respond to them.

Both apps function mainly by calling an API, served by a web server written in Go and hosted on AWS.

By the end of the project, I had a fully working system which was ready to be put into use. While I didn't have time to include every single feature I wanted, the end result is a usable beta version. Part of the reason for not ending up with a more fully featured app is the amount of work that went into design, testing, and dev ops, which all made up a significant part of the final project report.

The platform was created mainly for the purposes of this summer project, but also because I thought it was something that could be really useful. I'm hoping to continue working on it in the future.
