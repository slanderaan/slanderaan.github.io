---
layout: post
title:  "How this site was created"
date:   2025-03-01 11:58:21 -0500
categories: Guide
---
This site was setup with the following commands:

# PC PowerShell
winget install RubyInstallerTeam.Ruby.3.2
winget install RubyInstallerTeam.RubyWithDevKit.3.2

# Github setup
git config --global credential.helper manager-core

# Terminal
gem install jekyll bundler
jekyll new slanderblog

# Editor
navigate to slanderblog/\_posts
rename [date]-welcome-toj-jekyll.markdown to [date]-how-site-was-created.markdown
open /\_posts/[date]-how-site-was-created.markdown

# Github
cd slanderblog
git init
git add .
git commit -m "Initial Jekyll site"
git branch -M main
git remote add origin https://github.com/slanderaan/slanderaan.github.io.git
git push -u origin main
