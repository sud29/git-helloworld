Steps for creating New Repository.

1. Go into the directory containing the project.
2. Type git init.
3. Type git add to add all of the relevant files.
4. You’ll probably want to create a .gitignore file right away, to indicate all of the files you don’t want to track. Use git add .gitignore, too.
5. Type git commit to commit in local repository.

Once project is added to local repository, follow below instructions to add it to GitHub.com

1. Go to github.
2. Log in to your account.
3. Click the new repository button in the top-right. You’ll have an option there to initialize the repository with a README file, but I don’t.
4. Click the “Create repository” button.
5. Now, follow the second set of instructions, “Push an existing repository…”

$ git remote add origin git@github.com:username/new_repo
$ git push -u origin master

Actually, the first line of the instructions will say

$ git remote add origin https://github.com/username/new_repo

But I use git@github.com:username/new_repo rather than https://github.com/username/new_repo, as the former is for use with ssh (if you set up ssh as I mentioned in “Your first time”, then you won’t have to type your password every time you push things to github). If you use the latter construction, you’ll have to type your github password every time you push to github.