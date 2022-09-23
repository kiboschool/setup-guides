# Setup Git and Github

Watch a video of this walkthrough ([Windows](https://www.loom.com/share/3d455cc0b40a473cbc4dca356dfd9bf5))

## Sign up for a Github Account

Navigate to https://github.com/join and sign up for a Github account. Store your credentials in your _password manager_ (you should do this for all new logins).

If you already have a GitHub account, you can skip this step.

## Configure Git

Open your terminal (Cmder or Iterm2) and configure your name and email settings for Git.

```sh
git config --global user.email "you@example.com"
git config --global user.name "Your name"
```

Git will use these settings to attribute you as the author of any code that you write.

**Important**: Replace 'you@example.com' with the email address you used to sign
up for Github, and 'Your name' with your name (not your Github username -- the
name you'd like people to see when they check who authored some code).

## Connect Github your computer

You need to connect Git on your computer to your Github account.

To do this, you'll set up a pair of matched SSH keys on your computer, and share 
one of the keys with Github. When you connect to Github in the future, you won't
need to type in your username or password, because it will check who you are
using the key.

### Create an SSH key

Open a terminal (Cmder or iTerm2) and copy and follow the instructions below to
create an SSH key and connect it to Github.

**Important**: Be sure to use the email you used to sign up for Github.

```shell
ssh-keygen -t ed25519 -C "your_email@example.com"
```

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

```shell
> Enter a file in which to save the key (/c/Users/you/.ssh/id_algorithm):[Press enter]
```

Next, it will prompt you for a passphrase. **Do not enter a passphrase.**

Press Enter without typing a passphrase, then press Enter again at the second
prompt.

```shell
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]
```

The program will tell you that it created a pair of keys, and give the paths to those files. Note the path to the public key, because you'll need it in the next step. It should be something like:

Windows:
```
Your public key has been saved in C:\Users\user\.ssh/id_ed25519.pub
```

Mac:
```
Your public key has been saved in /Users/user/.ssh/id_ed25519.pub
```

### Copy your key

Now, you need to copy the key so that you can add it to Github. The `clip` or `pbcopy` command will copy the contents of the file to the clipboard, so that you can paste it into Github in the next step. 

(If you get a 'File not found error', use the file path from the previous step instead of the file paths shown in these examples)

Windows:
```powershell
clip < ~/.ssh/id_ed25519.pub
```

Mac:
```shell
pbcopy < ~/.ssh/id_ed25519.pub
```

### Add your key to Github

(borrowed from these [Github instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account))

- Navigate to Github in your browser
- In the upper-right corner of any page, click your profile photo, then click Settings.
- In the "Access" section of the sidebar, click  SSH and GPG keys.
- Click New SSH key or Add SSH key.
- In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal Dell Windows laptop, you might call this key "Personal Dell".
- Paste your key into the "Key" field.
- Click Add SSH key.

Github may ask you to enter your password again.

### Test your connection

To test that the keys and connection worked, enter this:

```sh
ssh -T git@github.com
```

You may see a warning like this:
```
> The authenticity of host 'github.com (IP ADDRESS)' can't be established.
> Ed25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU
> Are you sure you want to continue connecting (yes/no)?
```

Check that the fingerprint matches, then type 'yes' and press Enter.

If everything works, you'll see:
```shell
> Hi username! You've successfully authenticated, but GitHub does not
> provide shell access.
```

In the future, that means you can use SSH to interact with Git, and you won't
need to type your Github password into the Terminal.

## Read more about SSH 

Github has lots more information about SSH, Git, with options and tips for use.

1. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh
2. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
3. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account
4. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection

