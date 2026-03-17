# test-projects
Networking

# 1) Create an empty repo on GitHub named jacky-portfolio (private)

# 2) Unzip and go to the project root
unzip jacky-portfolio.zip
cd jacky-portfolio

# 3) Create a private repo called jacky-portfolio and push the current folder
gh repo create jacky-portfolio --private --source=. --remote=origin --push

# 4) Update badges to point at your repo and commit the change
OWNER=<your-github-username>
REPO=jacky-portfolio
OWNER=$OWNER REPO=$REPO bash shared/scripts/bash/update-badges.sh

git add -A
git commit -m "chore: set CI badges to actual repo"
git push
