# Academic Software and Accounts

Watch a video walkthrough of this guide ([Windows](https://www.loom.com/share/6eee1778693e4e4bb3b8ed377ebd5755))

There is also some general-purpose software you'll use throughout your academic
program. You may already have this software installed, so skip any applications
that you already have.

For each program, use the package manager (Scoop,
Homebrew, or Apt) for your operating system to install the software (examples 
for Windows using `scoop` are provided.)

## 1. Zoom 
Zoom is like a virtual gathering space where you can connect with your live classes, meet up with classmates, and have face-to-face conversations from the comfort of your own screen.


```powershell
scoop install zoom
```

<!-- 
For MacOS:
```sh
brew install --cask zoom
``` -->

## 2. Discord
Discord is like the ultimate hangout spot where you can chat, voice call, video call, and collaborate with your crew all in one place.

```powershell
scoop install discord
```

<!-- For MacOS
```sh
brew install --cask discord
``` -->

## 3. Google Chrome Browser

Google Chrome is like that trusty buddy who always has your back when it comes to surfing the web, loading pages in a flash and keeping things simple and smooth.

```powershell
scoop install googlechrome
```

<!-- For MacOS
```sh
brew install --cask google-chrome
``` -->

## 4. Password Manager

As a technologist, you will become responsible for critical accounts and software. That means that your personal security habits, including passwords, are an important skill to develop and practice.

One primary means of protecting your online security is to use a different and strong
password for every service.  But how do you remember all those complicated passowrds?  You use a Password Manager! We recommend _Bitwarden_ as an excellent free tool, but there are other effective tools too, especially if you are willing to pay. (Dashlane, 1Password, and LastPass are all acceptable).

If you already use a Password Manager, you can skip these steps. We **strongly encourage** that you use a Password Manager for all your passwords, instead of trying to remember them.

 1.  Create a Bitwarden account at [www.bitwarden.com](https://vault.bitwarden.com/#/register). Write down your master password on paper and keep it somewhere handy, but safe.  Remember to use a very strong master password.  If anyone were to get access to this account, they would have access to all your accounts!  More information on creating strong passwords is available from the [Cybersecurity & Infrastructure Security Agency](https://www.cisa.gov/news-events/news/choosing-and-protecting-passwords).
 2. Install Bitwarden 
 ```powershell
scoop install bitwarden
```

<!-- For MacOS
```sh
brew install --cask bitwarden
``` -->

3.  Install the Bitwarden browser extension by visiting [www.bitwarden.com/download/](https://bitwarden.com/download/) from your Chrome Browser

Now that you have a safe place to store your passwords, do the following:
* Add passwords to your most common accounts to Bitwarden.
* As you create new accounts, including for Kibo, use Bitwarden to generate and store a strong password. Don't think of your own passwords.

## 5. Consistent Usernames

Over time, it's helpful to build a consistent digital identity, so that people
can recognize your profile on different platforms.

Part of your 'personal brand' has to do with your usernames and handles. Tech
culture (rightly or wrongly) uses things like github and twitter handles as a 
status marker or indicator of being in the 'in' crowd.

It's not _necessary_ to think about curating your online persona this way, but
since you are likely to keep these accounts for a long time, it might be worth
thinking about now.

**What makes a username good?**

Here's some things that can be good. There aren't real rules for this, so treat
them more as suggestions.

- use the same username across platforms (Github, Linkedin, and social media)
- use the same profile picture
- consider using your name, or part of it, if it's available
- shorter is (usually) better
- use lowercase and remove spaces

**Example: Ope**

Kibo CEO Ope uses her name as her handle across different platforms, and uses
the same profile picture. That makes her easy to identify when encountering her
on a different site, which tends to make her personal brand stronger:

- https://www.linkedin.com/in/opebukola/
- https://twitter.com/ope_bukola
- https://github.com/opebukola
- https://replit.com/@opebukola

She goes one step further and also has https://opebukola.com/. We'll talk about domains later on. 

For now, just be aware that using a consistent username across different
accounts can be a positive signal in some tech spaces.

[Return to the README](./README.md)