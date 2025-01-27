
# Git Deployment

## Setup
https://docs.cpanel.net/knowledge-base/web-services/guide-to-git-set-up-deployment/

- Created fcc-projects repo via CPanel
- Repo has file ``.cpanel.yml`` for deployment
- cloned repo https://github.com/pythonadventurer/fcc-projects.git using CPanel Git tool

### Git Push to Multiple Repos
https://stackoverflow.com/questions/14290113/git-pushing-code-to-two-remotes


### Added both CPanel repo and Github repo as "origin
```
git remote set-url --add --push origin ssh://bluebykk@bluegatoronline.com:21098/home/bluebykk/repositories/fcc-projects        
git remote set-url --add --push origin https://github.com/pythonadventurer/fcc-projects.git
```

- Added ssh keys to C:\Users\robtf\.ssh

