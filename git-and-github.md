# Setup Git and Github

## Sign up for a Github Account

Navigate to https://github.com/join and sign up for a Github account. Store your credentials in your _password manager_ (you should do this for all new logins).

If you already have a GitHub account, you can skip this step.

## Configure Git

Open your terminal (Cmder or Iterm2) and configure your name and email settings for Git.

```sh
git config --global user.email "you@example.com"
git config --global user.name "Your name"
```

**Important**: Replace 'you@example.com' with your email, and 'Your name' with
your name! Git will use these settings to attribute you as the author of any code that you write.

## Configure SSH

You need to connect Git on your computer to your Github account.

Follow the steps on these pages to configure this authentication.

1. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
2. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account
3. https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection

