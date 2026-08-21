# Troubleshooting Git Push Errors
## Overview
This guide explains how to troubleshoot common problems that can occur when pushing changes to GitHub.
## Problem
You run:
```bash
git push
```
but Git returns an error.
## Common Causes
### 1. You are not connected to the internet
Git needs an internet connection to communicate with GitHub.
**Solution:** Check your internet connection and try again.
### 2. You are not authenticated
GitHub requires you to authenticate your account before you can push changes.
**Solution:** Sign in to GitHub or authenticate Git credential manager.
### 3. Your local branch is behind
Another change may have been pushed to the remote repository.
**Solution:** Run:
```bash
git pull
```
Then try:
```bash
git push
```
## Verification
After running `git push`, check the terminal for a successful message such as:
```text
main-> main
```
This indicates that your local changes were pushed to the remote repository.
## Tips
- Check your internet connection before troubleshooting Git.
- Read the error message carefully.
- Make sure you are working on the correct branch.
- Avoid repeating commands without understanding the error.
## Conclusion
Understanding common Git push errors makes it easier to troubleshoot problems and work confidently with GitHub.