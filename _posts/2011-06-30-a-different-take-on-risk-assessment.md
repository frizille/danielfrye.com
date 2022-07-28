---
id: 5
title: A Different Take on Risk Assessment
date: 2011-06-30T21:34:09+00:00
author: Daniel
layout: post
guid: http://www.fuzzdot.com/?p=5
permalink: /2011/06/30/a-different-take-on-risk-assessment/
categories:
  - Info Sec
tags:
  - risk assessment
  - security
---
First off, this is long winded, bear with me while we cover some foundational concepts first…

A few weeks ago I was asked to present alongside [Splunk](http://www.splunk.com/) at the [Gartner Security & Risk Management Summit in Washington DC](http://www.gartner.com/technology/summits/na/security/) as one of their customers and offer a view into how we’re using Splunk. Just having purchased Splunk and starting our implementation a few months ago, I wasn’t quite sure exactly how we would present a true “success story” as we’re still very much in the deployment phases of the product. After a couple days of thought, I settled on presenting Splunk as a strategic direction for our Risk Assessment methodology rather than on the technical aspects of our solution. With hindsight being 20/20 that was probably the right move; the audience at the Gartner Summit was much more on the management side than the technical side.

Now fast forward a few weeks to the Summit itself and a presentation by Dr. Eric Cole of [Secure Anchor](http://www.secure-anchor.com/) and [Core Security](http://www.coresecurity.com/). In Dr. Cole’s presentation (he’s a fantastic speaker by the way) one point he brought up that really hit a cord with me was this: **_organizations who are being breached are buying, and using, the same products as those who were not being breached_**. His argument was organizations properly leveraging the <span style="text-decoration: line-through;">products</span> tools they’ve purchased to decrease evaluated risk within the context of their business were the ones who were successful in defending their networks. Read that last sentence again to make it sink in.

This is an important point because it brings up the philosophy of Risk Assessment – **_you must truly understand and put context into your risk assessments to make them actually usable_**. So what do we mean by context? Well, let’s say you have a large consultant driven organization where most corporate users are mobile road warriors and a smaller back office staff at the corporate headquarters. Implementing an expensive Web Proxy solution does very little for your total risk of data loss as most users aren’t in the office. Conversely, focusing your limited budget on mobile solutions such as whole disk encryption or sensitive data scanning tools to make sure PID/CC#’s aren’t making it onto those mobile devices in the first place is a much better spend of the money; you’re stretching your dollars further to reduce more risk. Compared to a traditional brick and mortar office environment the exact opposite is true; the web proxy solution is a much better investment since it’s fairly uncommon for offices to be burglarized (note, I said uncommon, not impossible). The root risk is the same, i.e. data loss, but the technical evaluation of how to mitigate the risk is much different. As information security leaders we have to be able to place ourselves within the context of our own organizations to develop the correct tasking orders.

Now with those two understandings in place we can get to the root of this article. As information security leaders, even if it’s not in our official job description, we should always be evaluating where risks are within our enterprise and our business processes. But our risk assessment process, if we have one, is usually a paper-trail-mess of half completed frameworks. While the intent of the frameworks is noble, and they encompass a lot of areas we need to look at, it’s just takes too many resources to really do it the way the framework lays out. ALE, SLE? Forget it. They both rely on probability – a probability we cannot predict adequately; we are not insurance companies with actuary tables to refer to, and we won’t ever get there. Some things just cannot be predicted – human nature + business processes + computer vulnerabilities? Not even one of those things is predictable so why would we expect to believe we can predict monetary losses from them?

## Automating Operational Risk

So if our paperwork methods of risk assessment are too cumbersome, what do we do? The answer is ingrain risk assessment into our daily operational processes. Take a look at the Visio below.

[<img loading="lazy" class="aligncenter size-full wp-image-6" title="sec_process_flow" alt="" src="http://danielfrye.com/wp-content/uploads/2011/06/sec_process_flow.jpg" width="368" height="442" srcset="http://danielfrye.com/wp-content/uploads/2011/06/sec_process_flow.jpg 368w, http://danielfrye.com/wp-content/uploads/2011/06/sec_process_flow-250x300.jpg 250w" sizes="(max-width: 368px) 100vw, 368px" />](http://danielfrye.com/wp-content/uploads/2011/06/sec_process_flow.jpg)Conceptually the process, and I’m open to comments obviously, attempts to take the tools we use on a daily basis now and put them into a manageable, yet automated, framework. The process looks something like this:

  1. Nmap scans the network for active hosts and ports (Network Asset Inventory) then…
  2. … passes the network ranges with the active hosts flagged to our Nesses scanner (Software Versioning and Patch Status) which runs a vulnerability check and pulls the patch status on the box…
  3. … then does another Nessus check to validate the server is configured according to our hardening standards (Hardening & Configuration Data).

What that process essentially does is create an automated model for evaluating the traditional Risk equation we all know and love.

<p style="text-align: center;">
  <strong><em>THREAT x VULNERABILTY = RISK</em></strong>
</p>

The first box, providing our IPS, HIDS, and AV data is where we evaluate **_THREAT_** in the equation above for our environment. I’m not saying that since we have Apache webservers and we’re seeing IIS attacks that we’re not at risk, not at all. What I’m saying is that we can evaluate risks such as “we can be attacked via the internet on port 80/443 (and are) so we need to look at what additional processes need to be put into place to protect us in the future”. It also makes a good argument for the operations teams to keep their servers patched. Show them the attacks for the last day, month, or year and demonstrate the why. Don’t rely on “well, you can be attacked”. Show them. You’ll win more battles there, trust me.

The other three boxes outlined above demonstrate how we evaluate our level of **_VULNERABLITY_**. If the boxes are patched, appropriately hardened, and up then we’re good to go. We’ve proactively done everything within our power to reduce risk as much as we can since we have almost no control over the specific types of threats we encounter.

You’ll notice I didn’t use too many specific tools examples above – I’ll explore that in further blog posts; right now I’m just trying to portray the vision of what we’re doing.

So that’s the intro to Operational Risk… next post will be on how we boil that into Total Enterprise Risk. And yeah, some radical stuff there too. Probably.

Daniel