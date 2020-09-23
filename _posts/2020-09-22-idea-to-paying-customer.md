---
layout: post
title: Idea to paying customer in one month
description: A month ago I ran into a problem. One week later I solved it. And three weeks after that I turned it into a (tiny) business.
date: 2020-09-22
image: https://www.mugshotbot.com/m?theme=two_up&image=d33ff6b7&color=green&url=https://masilotti.com/idea-to-paying-customer
permalink: idea-to-paying-customer/
category: masilotti.com
---

When I get something in my head I dive in. And I dive deep. For example, a month ago I ran into a problem. One week later I solved it. And three weeks after that I turned it into a (tiny) business.

Here’s how I went from an idea in a notebook to my first paying customer. In 31 days.

{% include timelines/mugshot-bot.html %}

## The problem

It started when I was finishing up a [blog post]({% post_url 2020-08-12-test-deep-links-with-ui-testing %}). I had everything ready: the article was proof read, the code samples were in place, and a gist was uploaded to GitHub.

But I forgot about the social share image. You know, the little preview that pops up when you tweet a link.

![Twitter card preview for blog post](/images/twitter-card.png)

I spent *forever* trying to find the perfect stock photo. I tried all the "no design" tools to create one in my browser. Some were OK, a few were good, but most were just plain *generic*.

So I vowed to never waste another second generating these images.

## The process

What follows is a day-by-day overview of what I worked on and important milestones in building up the implementation.

### Day 1: The idea

What if I could automate all my social share images? Instead of futzing with a tool, I wanted to just drop a URL on my page and have that generate a decent looking preview.

So I jotted some notes for a MVP. What’s the absolute least I could build to get market validation?

![Notes for Mugshot Bot on August 18, 2020](/images/notebook.jpeg)

If you can’t read my chicken scratch most of those notes touch on three basic pieces of functionality.
1. Scrape a website for the `og:title` and `og:description`
2. Render an HTML view with a fixed design and drop in the scraped content
3. Convert to an image and host it

Turns out, if I kept the scope very narrow I could get something built pretty quickly. And so [Mugshot Bot](https://www.mugshotbot.com?utm_source=masilotti.com) was born.

### Day 2: `rails new`

Ah, the most exciting part of a project, creating a new app!

I spent the better part of the next few days heads down getting something working. Rails, Active Storage, and `wkhtmlto*` were all key players in being able to build something so quickly.

Having a hyper-focused scope encouraged me to work on only what mattered. There was no pressure to make things look pretty yet, just get it working.

### Day 4: Launch the MVP

Three days later I had something working. It was ugly and there was no landing page, but it worked.

<img src="/images/mugshot-bot-v1.jpeg" alt="v1 of Mugshot Bot" class="shadow-lg" />

I [tweeted](https://twitter.com/joemasilotti/status/1296089448942379008) asking for beta testers and discovered a few folks who were interested in helping. A few DMs later and the images were live on three different blogs!

I also [posted to Hacker News](https://news.ycombinator.com/item?id=24335060) with low expectations. But I made it to the top of the second page and generated over 2000 clicks.

### Days 5-21: Gather feedback, improve, rinse and repeat

The next two weeks were spent talking to as many people as possible to ask as many questions as they would answer.

I learned a lot of valuable information, including what to call these little images. Most importantly, people were excited. Turns out I wasn’t the only one running into this problem.

During this time I also built out a landing page to test copy. This was helpful in learning how people describe the problem.

<img src="/images/mugshot-bot-landing.jpeg" alt="Mugshot Bot landing page v1" class="shadow-lg" />

Every feature from here on out has come from (potential) customer feedback. This was an important learning because I usually build things where I'm the only customer.

### Day 22: Launch customizations

The most requested feature by a long shot was customizations. Bloggers wanted to make their social share images look like their own, with their own branding.

![v2 of Mugshot Bot](/images/mugshot-bot-v2.png)

So I added [Clearance](https://github.com/thoughtbot/clearance) for authentication and launched `/customize`, a single form to change a variety of settings. Now bloggers could change the accent color, the background pattern, and even upload a branded image for one of the themes.

Simple, on purpose. Because that's exactly what folks had asked for.

### Day 31: First paying customer!

I spent all day Saturday at [Weekend Club](https://www.weekendclub.co?utm_source=masilotti.com), an Indie Hacker accountability community. Even though I had to start early (5am EST!) I was able to finish up the Stripe integration and create a Pro plan for exclusive themes.

I received a ton of valuable feedback throughout the day. Everything from design tweaks to UX pointers to newsletter recommendations. And before the end of the day, **BOOM**! Someone saw enough value in the product to start paying for the Pro features.

## The takeaways

I'm a developer at heart. I love to build things. But I spent *more than half* of the month talking to potential customers.

It took just 3 days to build an MVP. I could have spent 3 months building something that was "better" but with zero market fit.

It's easy to read books and learn how important this step is in building a product. But to actually *live* it is mind blowing. And the results speak for themselves.

### Looking forward

In no way is this journey complete. Hell, it's only the beginning.

<a href="https://www.mugshotbot.com?utm_source=masilotti.com">
  <img src="/images/mugshot-bot-v3.jpg" alt="v3 of Mugshot Bot" class="shadow-lg rounded-lg" />
</a>

Acquiring a customer is one of the most motivating things I've done since going independent. I've never been more excited about building something.

Watch this space for updates on [Mugshot Bot](https://www.mugshotbot.com?utm_source=masilotti.com) or sign up for my newsletter. Lots more is coming soon!