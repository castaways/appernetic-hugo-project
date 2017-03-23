+++
date = "2017-03-23T19:17:52Z"
title = "Message in a bottle"
draft = false

+++
Entrepreneurship is like being a castaway on a remote island like Robinson Crusoe or Bear Grylls where you are threatened to be eaten by Komodo varans, tribes and mosquitoes or wiped out by Volcano eruptions.  The first thing you have to do is find water, shelter and make a fire, then start networking with the local tribes.

## Message in a Bottle
I sent away a message in a bottle, but it was not very practical because I only had one bottle and this morning when I walked around the island it had floated back to the shore, so I set out to find a new method and have experimented with smoke signals.

In a real business situation, this could mean that the newsletter service you have chosen has UX issues, for example, TinyLetter had lots of that, and it did not work on a big 1920 x 1200 display. The code for the letters also looked horrible. I tried Mailjet, and a solution from Estonia both had issues with the email ending up in the spam folder and long waiting time after registration to verify my account. Then I got the suggestion to check out Paloma.se. It worked without any issues, and no email ended up in the spam filter.   

Except for getting a special assignment from the nearest tribes head honcho and a small Volcano break out, I also managed to set up a big sign called Castaway.gq. 

## Creating castaway.gq with SSL, hosting, CMS and image management
At [freenom.com][1] it is easy to get your domain name for free.
Go to Management Tools and select Nameservers. Select Use custom name servers and enter:

PAM.NS.CLOUDFLARE.COM

THEO.NS.CLOUDFLARE.COM

remove all the other.

![enter image description here][2]

Go to [cloudflare.com][3] 

Set up a free account if you don’t have one, then add your new domain by selecting +Add Site.

![enter image description here][4]

Make an A record for www that points to 192.30.252.153 and one to 192.30.252.154

Create a CNAME record with the name of the domain and the alias with the subdomain (www.castaway.gq) to have the domain point to www:

![enter image description here][5]

Now set up your GitHub account:

![enter image description here][6]

Verify your email address.

Go to Appernetic.io and log in with your Github account and Authorize application.

Now you can setup your static website project

I selected the Hugo Future imperfect theme: https://github.com/jpescador/hugo-future-imperfect

It is a bit imperfect, but as it is open source, it is easy to fix issues. Remember to also give a shout out to the theme developer, so he is aware of the imperfections and if you like the theme, give him a PR.

When you are ready with your project sync it with GitHub and point your domain to GitHub by creating a CNAME file in the appernetic-hugo-project root folder, then sync a last time and publish the site.

Now all should be setup, and you only have to wait for 24 to 48 hours to have the domain name propagate on the Internet.

{{< youtube y1q4WD4mNKA >}}


  [1]: https://freenom.com
  [2]: https://res.cloudinary.com/appernetic/v1490304494/enuujml5qo1kjo6xp1se
  [3]: https://cloudflare.com
  [4]: https://res.cloudinary.com/appernetic/v1490304584/jsz0u2en8k5yzbgsj33l
  [5]: https://res.cloudinary.com/appernetic/v1490304679/fbhk7ojcuijuc3pesx0q
  [6]: https://res.cloudinary.com/appernetic/v1490304735/hidmmwwviejywbgtdeh8
