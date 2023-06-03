---
title: Lambda Tea
date: 2017-12-01 19:00:00 -05:00
layout: projects/project
description: A self-serve boba machine built by hacking a mini-fridge. Lambda Tea was funded by Y Combinator for their Winter 2018 batch.
imgSrc: /assets/projects/boba/boba4.jpg
---

To build our prototype, we repurposed a refridgerator, used peristaltic pumps that were controlled by an arduino, and connected the arduino to a tablet running an android app that we built. The android app accepted payments through venmo and verified payments by communicating with a server on AWS through a websocket. In order to fulfillment payments, we hacked a deprecated venmo API.

It was basically "boba on tap".

For more information about this project, see [1](https://mitadmissions.org/blogs/entry/lambda-tea/), [2](http://lambdatea.com/).

After MIT's Sandbox Innovation Fund awarded us $1,000 to build a boba machine, we worked on our project every night from midnight to 2AM for a month. Our goal was to make our boba machine, which we named Lambda Tea, fully self-sufficient like a vending machine. When we completed the machine, we placed the boba machine in one of our dorm rooms and opened it up to the public 24/7. Anyone could walk up to it at any time, choose their boba flavor, venmo the Lambda Tea account, and vend boba into a cup.

A look at where the boba machine was located.

![boba 3](/assets/projects/boba/boba2.jpg)

I built the Android app that users interface with and the server on AWS to verify venmo payments, store data about purchases, and send alerts when the machine breaks down or needs refills, as well as the AWS server that processes the data and communicates with the app,

In order to set up the payment processing mechanism, I used a deprecated venmo API... using a key that someone leaked on Github. When new payment is been received, the server sends a message through a websocket to the tablet, allowing the arduino to turn on the peristaltic pumps so that the user can vend boba.

Here is a look inside the boba machine while we were testing different ingredients:

![boba 4](/assets/projects/boba/boba4.jpg)

# The friendos

The most important part of this project. Those people are Robert Henning and Jingwei Ma. I'm the girl with the bad dye job.

![boba 5](/assets/projects/boba/boba5.jpg)

# Results

Our machine was surprisingly popular. We dispensed over 500 cups of boba within a month and sold each cup for $3.50. 203 unique customers purchased Lambda Tea boba and 46 peoples purchased 4+ cups of boba within two weeks.

Later, we applied to Y Combinator, the most competitive startup accelerator to get into, and were funded $120,000 in exchange for 7% equity. Our batch in Y Combinator had a 1.5% acceptance rate, and we were the youngest team; the average age in our batch was 29, and we were 20. We took a leave of absence and stayed in San Francisco for 8 months to develop our company. However, we weren't prepared to drop out of MIT so we came back to school.
