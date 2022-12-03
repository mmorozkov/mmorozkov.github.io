---
title: "Matrix Has You"
date: 2022-12-03T19:00:00+02:00
draft: false
toc: false
images:
tags: 
  - privacy
  - security
---

I recently bought a new TV, and when I was setting it up, it prompted me to download an app to finish the installation, which already sounded awkward. But the was just a beginning: I could not expect that app would say that in order to continue finishing the installation of my TV, I needed to grant it full access to my location **ALWAYS**. It triggered me so much, and actually made me think how far down the rabbit hole with privacy (or should I say lack thereof) we are already. And is there a saving grace at all?!

![TV](../location-always.png)

**WARNING:** The content below may bring sense of hopelessness 😫

## Internet
Internet remembers pretty much anything about you: what sites you visited, how often and when, how much time spent, where clicked, and where you were staring at. Almost pretty much every single company out there stores gigabytes of info on you, and for the right price they would sell it to anybody. But if we were to appoint one biggest culprit, it definitely would be Google:
1. Google Chrome literelly has built-in trackers that log all your actions, location, IP address and then some more
2. [A recent study][0] found that Google's trackers are installed in the vast majority of the sites worldwide
3. All their services track every single bit of your activity. [Check out][1] what they have on you!
4. [Google pays dozens of billions of dollars][2] to remain default search engine on the iPhone and Mac. If paying Apple $15B seems reasonable to Google, chances are they're making much more off of the users' information they gather
5. By the way, have you noticed how Google auto-suggests you while writing emails, and those suggestions are spot-on? I'm curious how they'd be able to do so ***without*** reading my mail
6. If it's not enoough, how about [Google disclosing your personal information][3] to authorities and lawyers, including for civil cases, too?!

## Gadgets
Smart things are cool, smart devices and AI are making life easier, I agree. It's sad that there's a lot of strings attached:
1. That Apple company, that put a lot of emphasis on privacy in their marketing in recent years, actually tracks you, even when you specifically told them not to do so! Here's the most recent [research][4], that proofs that
2. Ever wondered how Siri/Alexa/Google Home work? Well, they listen for an activation phrase (like `Hey Siri`) to help you. Also recording and sendnig to their servers everything else they heard in the meantime 😰
3. Not enough? How about those companies actually allowing humans to listen to those recordings in order to improve their products understanding capabilities. All of those big tech companies (Amazon, Apple, and Google) [were caught doing so][5], some of them even don't really anonymize the data, so that it can be traced back to the actual owner of the smart speaker 😱

## Social Networks and Messengers
The third pillar of this "Holy Trinity" is definitely all those social apps that were intended to connect people around the world. Well, technically they do, but there's a lot of things their owners "forgot" to publicly disclose:
1. Two most popular messengers, owned by Meta, are notorious users' privacy offenders:
    - Up to 2020 both Facebook Messenger and WhatsApp [didn't use end-to-end ecnryption][6], which means that any message sent on Messenger could be seen or intercepted in **plain text**.
    - Remember [Cambridge Analytica][7]? In 2018 Facebook allowed a 3rd party access to users' personal data without their consent
    - Meta repeatedly turned in users' personal data to authorities upon their requests
    - Hackers constantly find backdoors and vulnerabilities in WhatsApp, that [allow to take control over the whole device][8]!
    - The full laundry list of WhatsApp's sins was once put together by [Pavel Durov][9]
2. TikTok has been under US government's scrutiny for several years now, and for a [good reason][10].
    - It's not clear, if they're disclosing users' personal data to Chinese authorities
    - Here's a brief summary of what they collect from their [privacy policy][11]: location, IP address, search history, messages and what you look at and for how long, device identifiers to track your interactions with advertisers, phone number and social network contacts, and finally all your user-generated content
3. [Instagram and Twitter also have had privacy issues][12]

## What now?!
It's really hard to grasp, but one has to put up with the fact that this is the world we're living in, where we're all products. Here's what might help to come to grips with this:
- Delete all the data Google has on you
- Install open source browsers that do not track you whatsoever, like [Brave][13] or [Vivaldi][14]
- Use privacy-friendly search engine, like [DuckDuckGo][15]
- Switch off tracking services in your phone and disallow apps to track you
- Stop using WhatsApp, stick to messengers that use end-to-end encryption
- Buy a VPN and private email with encryption
- Be cautious with smart devices, change settings of your voice assistance to activate on some action like a button press, instead of actively listening for an activation phrase
- Consider going 20 years back and having a Motorolla flip phone 😅

[0]: https://spreadprivacy.com/followed-by-ads/
[1]: https://myactivity.google.com/myactivity
[2]: https://www.forbes.com/sites/johanmoreno/2021/08/27/google-estimated-to-be-paying-15-billion-to-remain-default-search-engine-on-safari/
[3]: https://transparencyreport.google.com/user-data/overview?metric=users_accounts
[4]: https://gizmodo.com/apple-iphone-analytics-tracking-even-when-off-app-store-1849757558
[5]: https://www.forbes.com/sites/jeanbaptiste/2019/07/30/confirmed-apple-caught-in-siri-privacy-scandal-let-contractors-listen-to-private-voice-recordings/
[6]: https://crambler.com/truth-about-facebook-messenger-app-privacy/
[7]: https://en.wikipedia.org/wiki/Facebook%E2%80%93Cambridge_Analytica_data_scandal
[8]: https://www.techspot.com/news/82843-hackers-can-use-whatsapp-flaw-way-handles-video.html
[9]: https://telegra.ph/Why-WhatsApp-Will-Never-Be-Secure-05-15
[10]: https://www.cnet.com/news/tiktok-called-a-national-security-threat-heres-what-you-need-to-know/
[11]: https://www.tiktok.com/legal/page/row/privacy-policy/en
[12]: https://www.privacy-ticker.com/privacy-issues-on-twitter-and-instagram/
[13]: https://brave.com/
[14]: https://vivaldi.com/
[15]: https://duckduckgo.com/