#How to release a new version of a library

This doc describes how to release a new version of a javascript library.  

##Dependencies

- [git-extras](https://github.com/visionmedia/git-extras)
- grunt

##Flow

1. Do work and commit
2. `git changelog`
3. Update version in the changelog file
4. If its a bug fix, increment patch number, if its a new feature, increment minor number.
5. Review the commits and clean up to make more readable
6. Edit bower.json and update the version to match the changelog
7. run `grunt`
8. run `git diff` and verify everything looks good
9. run `git release {version}`
