# Git_assignment_HeroVired
GIT Assignment

Steps:

# Created the repository and cloned it to the local machine
# Creted new dev branch using cmd  - git branch dev
# Added the code given in the assignment section where the divide function bug was not fixed and the square root function was added as a comment.
# Then this code was merged into the main branch and it was released as version 1.

git checkout -b dev
git add .
git commit -m "Adding square root feature"

# Switch to the main branch
git checkout main

# Merge 'dev' into 'main'
git merge dev

# Create a version 1 release tag
git tag -a v1.0 -m "Version 1.0 release"

# Push changes and tags to the remote repository
git push origin main --tags

# Next step is to Implement a feature by creating a new branch called ‘feature/sqrt’.

# Create a new branch for the feature
git checkout -b feature/sqrt

# Add the ‘sqrt’ code to it by uncommenting the sqrt code and saving it to this branch.

# To work on bugs at same time

git checkout dev

# Fix the bug in the divide function
# Update the divide function in Calculator class

# Commit the changes
git add.
git commit -m "Fixing divide function bug"

# Switch back to the 'feature/sqrt' branch
git checkout feature/sqrt

# Merge the changes from 'dev' into 'feature/sqrt'
git merge dev

# After completing the feature implementation and ensuring that the application works correctly, create a pull request targeting the main branch.
#On GitHub, create a pull request from 'feature/sqrt' to 'main'.

# Switch to the 'dev' branch
git checkout dev

# Merge 'feature/sqrt' into 'dev'
git merge feature/sqrt

# Test the changes

# Switch to the 'main' branch
git checkout main

# Merge 'dev' into 'main'
git merge dev

# Create a version 2 release tag
git tag -a v2.0 -m "Version 2.0 release"

# Push changes and tags to the remote repository
git push origin main --tags


