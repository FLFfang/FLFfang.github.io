# 

# 提交文章git流程

hugo --theme=LoveIt --baseURL="https://FLFfang.github.io/" --buildDrafts

cd public

git init(第一次要)

git add .

git commit -m "message"

git remote add origin git@github.com:FLFfang/FLFfang.github.io.git

git push -u origin master
