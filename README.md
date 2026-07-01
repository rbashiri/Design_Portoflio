General workflow you can reuse every time:

Decide your starting situation
Case A: No local folder yet, but remote repo already exists
Case B: Local folder exists with files, remote repo already exists
Case C: No remote repo yet (brand new project)



Case A (best/safest for your situation)
Clone first, then add your files
Commands:
git clone https://github.com/rbashiri/PORTFOLIO_BUILD_md.git
cd PORTFOLIO_BUILD_md
copy your project files into this folder
git add .
git commit -m "Add project files"
git push


Case B (you already did this path)
If folder is already git-initialized, do not run init again
Connect local folder to remote, pull, then commit your files
Commands:
git remote add origin https://github.com/rbashiri/PORTFOLIO_BUILD_md.git
git fetch origin
git pull origin main
git add .
git commit -m "Add local files"
git push -u origin main
Case C (new project, no remote yet)
Start with init, first commit, then create remote and push
Commands:
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-new-repo-url>
git push -u origin main
