---
title: "FAQ"
description: Frequently asked questions. Why did you make this site? I made the code open-source to show everyone what was going on behind the scenes and to allow others to help improve the application.
extends: _layouts.master
section: body
---

<h1 class="w-full text-center">FAQ</h1>
<div class="w-full mt-4 mb-12">
  <div class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"></div>
</div>

- [Why is it called AnonAddy?](#why-is-it-called-anonaddy)
- [Why did you make this site?](#why-did-you-make-this-site)
- [Why should I use AnonAddy?](#why-should-i-use-anonaddy)
- [Do you store emails?](#do-you-store-emails)
- [What is a shared domain alias?](#what-is-a-shared-domain-alias)
- [What is a standard alias?](#what-is-a-standard-alias)
- [Can I use my own domain?](#can-i-use-my-own-domain)
- [Why should I use this instead of a similar service?](#why-should-i-use-this-instead-of-a-similar-service)
- [Is there a browser extension?](#is-there-a-browser-extension)
- [Is there an Android app?](#is-there-an-android-app)
- [Is there an iOS app?](#is-there-an-ios-app)
- [How do I add my own GPG/OpenPGP key for encryption?](#how-do-i-add-my-own-gpgopenpgp-key-for-encryption)
- [Are attachments encrypted too?](#are-attachments-encrypted-too)
- [Are forwarded emails signed when encryption is enabled?](#are-forwarded-emails-signed-when-encryption-is-enabled)
- [What if I don't want anyone to link ownership of my aliases together?](#what-if-i-dont-want-anyone-to-link-ownership-of-my-aliases-together)
- [Where is the server located?](#where-is-the-server-located)
- [What if I don't trust you?](#what-if-i-dont-trust-you)
- [What is the maximum number of recipients I can add to an alias?](#what-is-the-maximum-number-of-recipients-i-can-add-to-an-alias)
- [What happens when I delete my account?](#what-happens-when-i-delete-my-account)
- [Does this work with any email provider?](#does-this-work-with-any-email-provider)
- [How do I reply to a forwarded email?](#how-do-i-reply-to-a-forwarded-email)
- [Does AnonAddy strip out the banner information when I reply to an email?](#does-anonaddy-strip-out-the-banner-information-when-i-reply-to-an-email)
- [How do I send email from an alias?](#how-do-i-send-email-from-an-alias)
- [Will people see my real email if I reply to a forwarded one?](#will-people-see-my-real-email-if-i-reply-to-a-forwarded-one)
- [Can emails have attachments?](#can-emails-have-attachments)
- [What is the max email size limit?](#what-is-the-max-email-size-limit)
- [What happens if I have a subscription but then cancel it?](#what-happens-if-i-have-a-subscription-but-then-cancel-it)
- [If I subscribe will Stripe see my real email address?](#if-i-subscribe-will-stripe-see-my-real-email-address)
- [How do you prevent spammers?](#how-do-you-prevent-spammers)
- [What do you use to do DNS lookups on domain names?](#what-do-you-use-to-do-dns-lookups-on-domain-names)
- [Is there a limit to how many emails I can forward?](#is-there-a-limit-to-how-many-emails-i-can-forward)
- [Is there a limit to how many aliases I can create per hour?](#is-there-a-limit-to-how-many-aliases-i-can-create-per-hour)
- [How is my bandwidth calculated?](#how-is-my-bandwidth-calculated)
- [How many emails can I receive before I go over my bandwidth limit?](#how-many-emails-can-i-receive-before-i-go-over-my-bandwidth-limit)
- [What happens if I go over my bandwidth limit in a given month?](#what-happens-if-i-go-over-my-bandwidth-limit-in-a-given-month)
- [Can I login using an additional username?](#can-i-login-using-an-additional-username)
- [I'm not receiving any emails, what's wrong?](#im-not-receiving-any-emails-whats-wrong)
- [How do I know this site won't disappear next month?](#how-do-i-know-this-site-wont-disappear-next-month)
- [Is the application tested?](#is-the-appliction-tested)
- [How do I host this myself?](#how-do-i-host-this-myself)
- [Who's behind AnonAddy?](#whos-behind-anonaddy)
- [I couldn't find an answer to my question, how can I contact you?](#i-couldnt-find-an-answer-to-my-question-how-can-i-contact-you)

## Why is it called AnonAddy? {#why-is-it-called-anonaddy}

AnonAddy is short for "Anonymous Email Address". The word "Addy" is internet slang for email address, e.g.

> "My addy is being spammed. I should've kept it private."

## Why did you make this site? {#why-did-you-make-this-site}

I made this service after trying a few other options that do a similar thing. I was really interested in how they worked and loved the thought of protecting my real email addresses from spam.

I also wanted to address some issues with other services such as:

* Proprietary closed source code
* Adverts, analytics and trackers used on the sites
* No option to encrypt emails using a GPG/OpenPGP key
* No option for multiple recipients

I made the code open-source to show everyone what was going on behind the scenes and to allow others to help improve the application.

I use this service myself for the vast majority of sites I'm signed up to.

## Why should I use AnonAddy? {#why-should-i-use-anonaddy}

There are a number of reasons you should consider using this service:

* Protect your real email address from spam by simply deactivating/deleting aliases that receive unsolicited emails
* Identify who has sold your data by using a different email address for every site
* Protect your identity in the event of a data breach by making it difficult for hackers to cross-reference your accounts
* Prevent inbox snooping by encrypting all inbound emails using GPG/OpenPGP encryption
* Update where emails are forwarded without having to go through and change your email address for each site individually
* Reply to forwarded emails anonymously without revealing your true email address

## Do you store emails? {#do-you-store-emails}

No I definitely do not store/save any emails that pass through the server.

## What is a shared domain alias? {#what-is-a-shared-domain-alias}

A shared domain alias is any alias that has a domain name that is also shared with other users. For example anyone can generate an alias with the @anonaddy.me domain. Aliases with shared domain names must be pre-generated and cannot be created on-the-fly like standard aliases.

## What is a standard alias? {#what-is-a-standard-alias}

A standard alias is any alias that can be created on-the-fly. Automatic on-the-fly alias creation is only available for domains that are unique to you. For example, your unique username subdomain, any additional usernames or any custom domains. So if you signed up with the username "johndoe", any alias you create using @johndoe.anonaddy.com would be a standard alias (even if you've generated a UUID/Random Word one).

## Can I use my own domain? {#can-i-use-my-own-domain}

Yes you can use your own domain name so you can also have *@example.com as your aliases. To do so you simply need to add a TXT record to verify your ownership of the domain. Then you will need to add an MX record to your domain so that our server can handle incoming emails. You can then add a few other records to enable sending from your domain too.

## Why should I use this instead of a similar service? {#why-should-i-use-this-instead-of-a-similar-service}

Here are a few reasons I can think of:

* Bring your own GPG/OpenPGP key to encrypt your forwarded emails (and the option to replace subjects)
* No adverts
* No analytics or trackers (just server access logs)
* No third party content (excluding stripe.js on the subscription page)
* Open-source application code
* No limitation on the number of aliases that can be created
* Generous monthly bandwidth
* Multiple domains to choose for aliases (currently anonaddy.com, anonaddy.me and another for paid plan users)
* Ability to generate UUID and random word aliases at shared domains
* Ability to add additional usernames to compartmentalise aliases
* New features added regularly

## Is there a browser extension? {#is-there-a-browser-extension}

Yes there is an [open-source](https://github.com/anonaddy/browser-extension) browser extension available to download for [Firefox](https://addons.mozilla.org/en-GB/firefox/addon/anonaddy/) and [Chrome](https://chrome.google.com/webstore/detail/anonaddy/iadbdpnoknmbdeolbapdackdcogdmjpe) (also available on other chromium based browsers such as Brave and Vivaldi). You can use the extension to generate new aliases remotely.

## Is there an Android app? {#is-there-an-android-app}

There is not an official Android app that I have made myself as I am not familiar with mobile development.

There is however an excellent [open-source](https://gitlab.com/Stjin/anonaddy-android) Android app created by [Stjin](https://twitter.com/Stjinchan) that is available to download from the [Play Store](https://play.google.com/store/apps/details?id=host.stjin.anonaddy) (paid) and [F-Droid](https://f-droid.org/packages/host.stjin.anonaddy) (free). The developer of this app has put in a lot of time and effort so if you would like to support him please purchase the Play Store version.

There is also another unofficial [open-source](https://github.com/KhalidWar/anonaddy) Android app created by [KhalidWar](https://twitter.com/RealKhalidWar) available from the [Play Store](https://play.google.com/store/apps/details?id=com.khalidwar.anonaddy).

## Is there an iOS app? {#is-there-an-ios-app}

At the moment there is not an app available for iOS. I believe the developers above may be looking into creating one but there is no time scale on this. In the meantime please use the web application in your mobile's browser.

## How do I add my own GPG/OpenPGP key for encryption? {#how-do-i-add-my-own-gpgopenpgp-key-for-encryption}

On the recipients page you simply need to click "Add public key" and paste in your **public** key data. Now all emails forwarded to you will be encrypted with your key. You should also replace the subject line of forwarded messages in your account settings as this cannot be encrypted.

## Are attachments encrypted too? {#are-attachments-encrypted-too}

Yes attachments are part of the email body and are also encrypted if you have it enabled.

## Are forwarded emails signed when encryption is enabled? {#are-forwarded-emails-signed-when-encryption-is-enabled}

Yes when you have encryption enabled all forwarded emails are signed using our mailer@anonaddy.me private key.

You can add this key to your own keyring so that you can verify emails have come from us.

The fingerprint of the mailer@anonaddy.me key is <span class="break-words">"26A987650243B28802524E2F809FD0D502E2F695"</span> you can find the key on [https://keys.openpgp.org](https://keys.openpgp.org/search?q=26A987650243B28802524E2F809FD0D502E2F695).

## What if I don't want anyone to link ownership of my aliases together? {#what-if-i-dont-want-anyone-to-link-ownership-of-my-aliases-together}

If you're concerned that your aliases are all linked by your username e.g. @johndoe.anonaddy.com, then you have a couple of options:

1. You can generate UUID or random word aliases instead, these are all under a shared domain and cannot be linked to a user.
2. You can add additional usernames and separate your aliases under your these. e.g. you could have one username for personal stuff, another for work, another for hobbies etc.

## Where is the server located? {#where-is-the-server-located}

The server is located in Amsterdam, Netherlands with [Greenhost.net](https://greenhost.net/). Greenhost focuses greatly on privacy and security and their servers run entirely on Dutch wind energy.

## What if I don't trust you? {#what-if-i-dont-trust-you}

It's good to keep your guard up when online so you should never trust anyone 100%. I'll try my best to be as honest and transparent as I can but if you still aren't convinced you can always just fire up your own server and self-host this application. You'll need to know about server administration and PHP. You can find more information [here](/self-hosting).

## What is the maximum number of recipients I can add to an alias? {#what-is-the-maximum-number-of-recipients-i-can-add-to-an-alias}

The limit is currently set to 10 which should suffice in the vast majority of situations.

## What happens when I delete my account? {#what-happens-when-i-delete-my-account}

When you delete your account the following happens:

* All of your recipients are deleted from the database
* All of your aliases that use a shared domain e.g. @anonaddy.me are soft deleted from the database (this is to prevent any chance of another user generating the same alias in the future)
* All of your other aliases are deleted from the database
* All of your custom domains are deleted from the database
* Your user details are deleted from the database
* Your username and any additional usernames that you created are encrypted and added to a table in the database. This is to prevent anybody signing up with the same username in the future.
* Any subscription information is deleted from the database

## Does this work with any email provider? {#does-this-work-with-any-email-provider}

Yes this will work with any provider, although I can't guarantee it won't land in spam initially.

## How do I reply to a forwarded email? {#how-do-i-reply-to-a-forwarded-email}

Each forwarded email has a From: header set. This header will look something like this:

From: <span class="break-words"><alias+hello=example.com@johndoe.anonaddy.com></span>

Where hello@example.com is the address of the person who sent you the email and alias@johndoe.anonaddy.com is the alias that forwarded you the email.

All you need to do is click reply in your email client or web interface and it will automatically fill the To: field with the correct address.

To check if a reply has worked properly check in your dashboard if the reply count has been incremented for that alias.

For further details please see this help article - [Replying to email using an alias](https://anonaddy.com/help/replying-to-email-using-an-alias/).

## Does AnonAddy strip out the banner information when I reply to an email? {#does-anonaddy-strip-out-the-banner-information-when-i-reply-to-an-email}

At the moment the site does not automatically strip out the "This email was sent to..." text from forwarded emails when you reply to them. You need to either remove this from the quoted text manually or set the banner information to "off" in your account settings.

## How do I send email from an alias? {#how-do-i-send-email-from-an-alias}

This works in the same way as replying to an email.

Let's say that you have the alias **first@johndoe.anonaddy.com** and you want to send an email to **hello@example.com**.

All you need to do is enter the following in the To: field.

<span class="break-words"><first+hello=example.com@johndoe.anonaddy.com></span>

> **Note**: you must send the email from a verified recipient on your account.

Then send the email exactly as you would any other. To check that the email has sent successfully, look in your dashboard at the sent count column and see if it has been incremented for that alias.

If you want an easy way to construct the correct email address that you should send to you can click "Send from" next to any alias in the web application and after entering the destination address it will display the right email address to use.

This works exactly the same for shared domain aliases, additional usernames and custom domains.

You can even use the send from feature to create an alias on the fly that does not yet exist. This only works for standard aliases or those at custom domains that behave as a catch-all.

You must generate aliases that use shared domains (e.g. circus.waltz449@anonaddy.me) beforehand in order to be able to send from them.

For further details please see this help article - [Sending email from an alias](https://anonaddy.com/help/sending-email-from-an-alias/).

## Will people see my real email if I reply to a forwarded one? {#will-people-see-my-real-email-if-i-reply-to-a-forwarded-one}

No, your real email will not be shown, the email will look as if it has come from us instead. Just make sure not to include anything that might identify you when composing the reply, i.e. your full name.

## Can emails have attachments? {#can-emails-have-attachments}

Yes you can add attachments to emails forwarded and replies. Attachments count towards your bandwidth.

## What is the max email size limit? {#what-is-the-max-email-size-limit}

The max email size is currently set to 10MB (including attachments).

## What happens if I have a subscription but then cancel it? {#what-happens-if-i-have-a-subscription-but-then-cancel-it}

If you cancel your subscription it will remain active until the end of your current billing cycle, you will still be able to use your paid plan features until the billing cycle ends.

A few days before your billing cycle ends you will receive an email letting you know the steps you need to take to prevent the loss of any emails. Shortly after ending the following will happen:

* Any custom domains will be **deactivated**
* Any additional usernames will be **deactivated**
* If you have any more than **2 recipients** they will be **deleted**
* Paid account settings will be reverted to default values
* Any aliases using paid plan only domains will be **deactivated**
* If you have any more than 20 aliases using a shared domain e.g. anonaddy.me they will be **deactivated**
* If your account username has catch-all disabled then it will be enabled

You will not be able to activate any of the above again until you resubscribe.

## If I subscribe will Stripe see my real email address? {#if-i-subscribe-will-stripe-see-my-real-email-address}

No, Stripe will instead be given an alias. This alias will only be created if Stripe sends an email to it, for example if your card payment fails or if your card has expired.

## How do you prevent spammers? {#how-do-you-prevent-spammers}

The following is in place to help prevent spam:

* Rspamd - Fast, free and open-source spam filtering system
* DNS blacklist checks - spamhaus.org
* SPF, DKIM - to check the SPF record on the sender's domain
* DMARC - to check for email spoofing and reject emails that fail
* FQDN - the sender must be using a valid fully qualified domain name
* PTR record check - if the sender has no valid PTR record it is rejected

## What do you use to do DNS lookups on domain names? {#what-do-you-use-to-do-dns-lookups-on-domain-names}

The server is running a local DNS caching server to improve the speed of queries.

## Is there a limit to how many emails I can forward? {#is-there-a-limit-to-how-many-emails-i-can-forward}

Not unless you are really going to town. Each user is throttled to 200 emails per hour through the server.

## Is there a limit to how many aliases I can create per hour? {#is-there-a-limit-to-how-many-aliases-i-can-create-per-hour}

Currently you are limited to creating 10 new aliases per hour on the free plan, 20 per hour on the Lite plan and 50 per hour on the Pro plan. If you try to create more than this the emails will be deferred until you are back below the limit.

## How is my bandwidth calculated? {#how-is-my-bandwidth-calculated}

Each time a new email is received Postfix calculates its size in bytes. A column in the database is then simply incremented by that size when the email is forwarded or a reply is sent. At the start of each month your bandwidth is reset to 0.

I don't use rolling 30 day total as the only way to do this would be to log the date and size of every single email received.

Blocked emails do not count towards your bandwidth (e.g. an alias is inactive or deleted).

## How many emails can I receive before I go over my bandwidth limit? {#how-many-emails-can-i-receive-before-i-go-over-my-bandwidth-limit}

The average email is about 76800 bytes (75KB), this is roughly equivalent to 7,000 words in plain text. So the 10MB monthly allowance would be around 140 emails and the Lite plan's 50MB would be almost 700 emails.

## What happens if I go over my bandwidth limit in a given month? {#what-happens-if-i-go-over-my-bandwidth-limit-in-a-given-month}

If you get close to your limit (over 80%) you'll be sent an email letting you know. If you continue and go over your limit the server will start discarding emails until your bandwidth resets the next month or you upgrade your plan.

## Can I login using an additional username? {#can-i-login-using-an-additional-username}

You can add 1 additional username as a Lite user and up to 3 additional usernames as a Pro user for totals of 2 and 4 respectively (including the one you signed up with). You can currently only login with the one that you originally signed up with.

## I'm not receiving any emails, what's wrong? {#im-not-receiving-any-emails-whats-wrong}

Please make sure to add mailer@anonaddy.me, mailer@anonaddy.com and any other aliases you use to your address book and also to check your spam folder. Make sure to mark emails from AnonAddy as safe if they turn up in spam.

If an alias has been previously deleted and you try to send email to it, the emails will be rejected with an error message - "554 5.7.1 Recipient address rejected: Access denied".

Check that you have not deactivated the alias, custom domain or additional username. When any of these are deactivated, emails will be silently discarded, they will not be rejected or return any error message.

The sender of the email may be failing SPF, DMARC or DNS blacklist checks resulting in the email being rejected. The sender should also have correct reverse DNS setup and use a FQDN as their hostname.

If you are forwarding emails to an icloud.com email address some users are having issues with a small number of emails being rejected (often those from Facebook).

For some reason Apple seems to think these emails are spam/phishing and returns this error message:

> Diagnostic-Code: smtp; 550 5.7.1 [CS01] Message rejected due to local policy.

I have contacted Apple multiple times about this but they have not yet responded.

If you are having issues with emails being rejected as "possibly spammy" by Google, iCloud or Microsoft then please try the following steps if you can:

1. **Replace the email subject** by going to your settings in AnonAddy
2. Try adding a GPP key and **enabling encryption**. This will prevent the email's content being scanned and reduce the change of it being rejected.

I will also soon be adding an option to change the format of the display from part of the "From:" header.

If neither of the above options work then please try changing to another recipient so that you can continue to recieve emails.

If you still aren't receiving emails please contact me.

## How do I know this site won't disappear next month? {#how-do-i-know-this-site-wont-disappear-next-month}

I am very passionate about this project. I use it myself every day and will be keeping it running indefinitely. The service also provides me with an income.

## Is the application tested? {#is-the-appliction-tested}

Yes it has over 180 automated PHPUnit tests written.

## How do I host this myself? {#how-do-i-host-this-myself}

You will need to set up your own server with Postfix so that you can pipe the received mail to the application. You can find more information [here](/self-hosting).

For those who prefer using Docker there is an image you can use here - [github.com/anonaddy/docker](https://github.com/anonaddy/docker).

## Who's behind AnonAddy? {#whos-behind-anonaddy}

My name is Will Browning, I'm a web developer from the UK and an advocate for online privacy and open-source software. You can find me on [Twitter](https://twitter.com/willbrowningme) although I don't tweet that much!

## I couldn't find an answer to my question, how can I contact you? {#i-couldnt-find-an-answer-to-my-question-how-can-i-contact-you}

For any other questions just send an email to - [contact@anonaddy.com](mailto:contact@anonaddy.com) ([GPG Key](/anonaddy-contact-public-key.asc))
