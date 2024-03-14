# 

title = 'Commit_posts_flow'
date = 2024-03-14T22:22:41+08:00
draft = true

# commit_posts_flow

hugo --theme=LoveIt --baseURL="https://FLFfang.github.io/" --buildDrafts

cd public

git init(第一次要)

git add .

git commit -m "message"

git remote add origin git@github.com:FLFfang/FLFfang.github.io.git

git push -u origin master
