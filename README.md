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
how to list tag 
git tag
git tag -l "v1.*"
git show-ref --tags
how to delet tag locally and remotly
Delete the local tag:
git tag -d <tag_name>
Delete Remotely:
git push origin --delete <tag_name>
Combined Command (Local and Remote):
git tag -d <tag_name> && git push origin --delete <tag_name>

Project Image

![Project Logo](https://www.20i.com/blog/wp-content/uploads/2022/08/git-blog-header.png)
