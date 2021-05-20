---
description: Frequently Asked Questions
---

# FAQ

## Feature Questions

### Can you add a feature for me?

Usually, yes. Just let me know. But there's a queue. I'm only one guy and FrontierNav doesn't pay enough for me to work on it a lot. This means new features will be added depending on how complicated it is, how often it's requested and how interested I am in it. Time is really the key metric here. If I had [enough donations](https://patreon.com/jahed) I could spend more time on FrontierNav and get more features added.

### Why doesn't this game have any data?

Currently, games are based on what an Admin is playing or plans to play. It doesn't mean there's a commitment to add any other information. FrontierNav's data is community-driven so if you would like to contribute data to help others, you're strongly encouraged to. See "[Making Changes](editing-data/making-changes.md)". This will be expanded in the future to let anyone add games and take ownership of data maintenance much like a Wiki.

### Why does FrontierNav only support a Dark Theme?

FrontierNav is made to be a companion while playing video games, so ideally it should be out of focus with the main focus being on the game. The easiest way to do this is to use a dark theme which reduces the amount of light emitted by displays which in turn prevents grabbing your attention when you're not focusing on it.

A Light Theme may be added in the future, but it's not a priority. Supporting both Light and Dark Themes is a lot of work when adding and re-designing features as it doubles the manual testing surface since there's no automated way to ensure colours look correct to the human eye.

### Why does it take so long to load some games?

FrontierNav is a very dynamic application. So to reduce server-side burden \(as I'm running on a budget\), your browser downloads the entire latest database for the game. This can be as little as a few kilobytes to a couple of megabytes depending on the game. After the initial download, your browser won't need to download it again until the database is changed.

### Why does the Email Login Link come from Firebase?

FrontierNav uses [Firebase](https://firebase.google.com/) to store user credentials. So the login link will be sent by them. To avoid spam, Firebase does not allow this email to be customised at all so it won't have FrontierNav's branding. But don't worry, it's safe. It contains a single link which will automatically log you in.

### Why can't I log in with a password?

To avoid dealing with account hijacking, weak passwords, phishing and general malicious intent, FrontierNav avoids using passwords. You can only login through other social media platforms or a login link sent through email.

If your social media or email account is hijacked, please resolve it with those providers as it's pretty much impossible for FrontierNav to validate your identity without them. FrontierNav takes monthly backups so if an account is hijacked, once you regain access, you can request any lost data to be restored.

### What's your data policy?

* Access logs are stored for 5 weeks for monthly audits of malicious activity.
* Error logs are stored for 1 month for troubleshooting and fixing issues.
* Login data \(such as emails, names and avatars\) are stored indefinitely.
* Application data \(such as game libraries and forum posts\) is stored indefinitely.
* Data backups are stored for 1 month in case of data loss.
* Application data may be visible to other users.
* No passwords are stored.
* All data is visible to admins for auditing and admin-related tasks such as account recovery and backups.
* You can request to remove any data you've submitted.

### Can I delete my account?

Yes, [contact me](https://jahed.dev/about).

## Development Questions

### How often is FrontierNav updated?

FrontierNav is updated constantly. There is no fixed release cycle. However, you can get weekly news of what's changed on [my blog](https://jahed.dev/tags/frontiernav).

### Why isn't FrontierNav open source?

Parts of FrontierNav [are open source](https://github.com/jahed); the parts that can be used in other projects. FrontierNav's data is open and available under "[Creative Commons Attribution-ShareAlike 4.0 International \(CC BY-SA 4.0\)](https://creativecommons.org/licenses/by-sa/4.0/)" which is common for wikis. You can [save the data](editing-data/making-changes.md#saving-changes) and it in your own applications within the terms of the license.

FrontierNav's codebase is not open source as it's experimental and there's an overhead in providing enough documentation for others to contribute code. FrontierNav was open source in the past, but due to a lack of contributions, the overhead wasn't paying off. FrontierNav may become open source again in the future if it can generate [enough donations to sustain such an endeavour](https://patreon.com/jahed).

