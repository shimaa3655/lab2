To remove branches locally and remotely in a Git repository, you can use the following commands:
# Delete a local branch
git branch -d branch_name
If the branch has not been merged, Git will prevent you from deleting it with the -d option. In that case, you can use -D:
# Force delete a local branch (even if not merged)
git branch -D branch_name
Remove Remote Branch:
# Delete a remote branch
git push origin --delete branch_name
# Delete a remote branch
git push origin :branch_name
Combine Local and Remote Removal:

If you want to delete a branch both locally and remotely in one command, you can use:
git push origin --delete branch_name
git branch -d branch_name
