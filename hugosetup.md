

git submodule add [repo link] themes/[folder name]

cd themes/[folder name]/exampleSite/

hugo serve  --themesDir ../..


to run locally: http://localhost:1313/


https://dev.to/dgavlock/creating-a-hugo-site-on-github-pages-3cjo

- install hugo as needed
- sign up github
- create a repo called [youre site name] with readme
- create a repo called [your github name].github.io with readme
- hugo new site [youre site name]
- cd [youre site name]
- git init
- git remote add origin [link from your repo named as your site name]
- git pull origin master
- vim .gitignore
- public/ -> esc, :wq
- git add .
- git status
- git commit -m "msg"
- git push origin master
- cd themes
- git clone [link to your hugo theme]
- rm -rf hugo-creative-portfolio-theme/.git
- cd [theme name]
- cd examplesite
- move all files (except: theme.toml README.md Makefile LICENSE.md) under [your site] foler
- edit config.toml: change baseurl as "https://[your github name].github.io/"
- move to your root folder (where your site name is)
- git clone [link from your github name.github.io repo]
- move to your site folder
- hugo -d ../yourgithubusername.github.io
- git add .
- git commit -m "your message"
- git push origin master
- move to yourgithubname.github.io folder
- git add .
- git commit -m "your message"
- git push origin master

