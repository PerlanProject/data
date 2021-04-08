# data
Data for the Perlan data website.  Includes per-flight data, balloon soundings, and more.

**This repo contains files > 100MB! Therefore, you must install the git "large files" extension.  
See https://git-lfs.github.com"**

# Installing Git Large File Storage (Mac)

```sh
# install (or download and manually install from https://git-lfs.github.com
$ brew install git-lfs

# Update global git config
$ git lfs install

# Update system git config
$ git lfs install --system

# In each Git repo where you want to use LFS, add the file types (or directly edit .gitattributes)
$ git lfs track "*.wav" # or whatever files you want

# Ensure .gitattributes is tracked
$ git add .gitattributes
```

Note that defining the file types Git LFS should track will not,
by itself, convert any pre-existing files to Git LFS, such as files
on other branches or in your prior commit history. To do that, use
the git lfs migrate[1] command, which has a range of options designed
to suit various potential use cases.

Now, just commit and push to GitHub as you
normally would.


