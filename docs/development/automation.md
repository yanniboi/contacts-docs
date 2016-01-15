#What are we automating?

##Tests

When a pull request to our github repo is created, we are using TravisCI to automatically test the changes.

[Read more](http://blog.freelygive.org.uk/)

##GitHub and Drupal.org Issues

Whe you are working on an issue. You should first create an issue on Drupal.org.

Next create a new branch out of 8.x-1.x of your decoupled_auth fork on Github. This branch should end in the issue number from drupal.org.
Eg. `git checkout -b issue-2636140`

Then when you create the pull request and everytime you push changes to it, it should automatically post a comment on the issue on Drupal.org with a patch file containing the work you have done.

This is done thanks to klausi's [Github Pull request to drupal.org synchronization](https://github.com/klausi/github_drupalorg)