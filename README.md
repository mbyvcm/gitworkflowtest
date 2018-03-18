### gitworkflow

1. Clone repository from AWGL github to local system using HTTPS. You will prompted to enter valid username / password.
```https://github.com/AWGL/<repository_name>.git```

This will automatically set up the AWGL repository as the 'origin' remote. This can be confirmed;

```
cd <repository_name>
git remote -v

output:
origin	https://github.com/AWGL/<repository_name>.git (fetch)
origin	https://github.com/AWGL/<repository_name>.git (push)
```

2. Create a new branch and adjust code within this branch

add new branch
``` git branch v2```

move to new branch
``` git checkout v2```

commit any code adjustments

3. Push new branch back to remote
``` git push origin v2```

4. Set up pull request for code review

This can be done using the github interface under the 'release' tab or using the command line:

```git request-pull v2 https://github.com/AWGL/<repository_name>.git  master```

5. Code review and merge new version into master

6. Tag new version using the github interface
