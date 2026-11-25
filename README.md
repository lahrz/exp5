# exp5
# exp5

Step 1: Create a local repository
Open Git Bash and execute:
mkdir experiment5
cd experiment5
git init -b main


Step 2: Create a source file and commit it
echo "This is my GitHub experiment" > app.txt
git add app.txt
git commit -m "Initial commit"
git log --oneline


Step 3: Create a remote repository on GitHub
1. Open https://github.com
2. Log in to your GitHub account.
3. Click the + icon in the top-right corner.
4. Select New repository.
5. Enter the repository name as experiment55.
6. Choose Public or Private.
7. Click Create repository.
Step 4: Connect the local repository to GitHub
Replace USERNAME with your GitHub username.
git remote add origin https://github.com/USERNAME/experiment55.git


Verify the remote repository:
git remote -v


Step 5: Push the local repository to GitHub
git push -u origin main


Open your GitHub repository and verify that app.txt is present.
Step 6: Create and switch to a feature branch
git checkout -b feature-branch


Verify the branch:
git branch


Step 7: Modify the source file in the feature branch
echo "Feature in a separate branch" >> app.txt


Stage and commit the changes:
git add app.txt
git commit -m "Add feature branch changes"
git log --oneline


Step 8: Push the feature branch to GitHub
git push -u origin feature-branch


Step 9: Create a Pull Request on GitHub
1. Open your repository on GitHub.
2. Select the feature-branch branch.
3. Click Compare & pull request.
4. Set the base branch as main.
5. Set the compare branch as feature-branch.
6. Enter the title: Add feature branch changes.
7. Click Create pull request.
Step 10: Merge the Pull Request
1. Open the created Pull Request.
2. Click Merge pull request.
3. Click Confirm merge.
4. Verify that the Pull Request has been merged successfully.
Step 11: Update the local main branch
Return to Git Bash.
git checkout main
git pull origin main


Step 12: Verify the final file content
cat app.txt


Expected output:
This is my GitHub experiment
Feature in a separate branch


Step 13: Display the commit history
git log --oneline


To view the graphical branch history:
git log --oneline --graph --all


Step 14: Verify the feature branch
git checkout feature-branch
git log --oneline

compare and pull request
create pull req
merge pull req
config merge
check app.txt
