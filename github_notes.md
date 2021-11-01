When seeing this error message:
```bash
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
```
follow this solution to configure git password with your personal token:
https://stackoverflow.com/questions/68775869/support-for-password-authentication-was-removed-please-use-a-personal-access-to

Once the new personal token has put in, click `Always allow` button to avoid entering the mac password every time when run git commands. 


### Edit github personal token once it get expired and update with keychain access
https://docs.github.com/en/get-started/getting-started-with-git/updating-credentials-from-the-macos-keychain
