Method 1 — Remove Stored Credentials (Most Common)

Run:

git config --global --unset credential.helper

Then delete stored credentials:

rm ~/.git-credentials
Method 2 — Remove GitHub Login from Credential Manager

If credentials are cached:

git credential-cache exit
Method 3 — Remove Authorization from GitHub Website

Go to GitHub

Click your profile picture

Open Settings

Go to Applications

Click Authorized OAuth Apps

Remove the Git authorization.

Method 4 — Remove Local Repository Remote (if you want to disconnect repo)

Inside your project folder run:

git remote remove origin

This disconnects your local repo from GitHub.

Check if GitHub Is Removed

Run:

git remote -v

If nothing appears, the repo is no longer connected.

✅ If you want, I can also show you how to switch GitHub accounts in Visual Studio Code without deleting everything, which many developers use when handling multiple GitHub accounts.