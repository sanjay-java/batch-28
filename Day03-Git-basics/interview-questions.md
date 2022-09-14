#### What is the difference between git pull and git fetch?
  git fetch only downloads new data from a remote repository, but it doesn’t integrate any of the downloaded data into your working files. All it does is provide a view of this data.

  git pull downloads as well as merges the data from a remote repository into your local working files. It may also lead to merge conflicts if your local changes are not yet committed. Use the git stash command to hide your local changes.
