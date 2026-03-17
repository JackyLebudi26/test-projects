
gh auth login

unzip jacky-portfolio.zip
cd jacky-portfolio

# set the remote to your existing repo
git init
git add .
git commit -m "feat: portfolio scaffold (support • network • cloud)"
git branch -M main
git remote add origin https://github.com/JackyLebudi26/test-projectsi.git
git push -u origin main

# update badges and push
OWNER=JackyLebudi26 REPO=test-projectsi bash shared/scripts/bash/update-badges.sh
git add -A
git commit -m "chore: set split CI badges to actual repo"
git push
