```
     _  ___   ___  ____
  __| |/ _ \ / _ \|  _ \
/  _  | | | | | | | |_) |
| (_| | |_| | |_| |  __/
 \___/ \___/ \___/|_|
```

Had enough of copy and pasting the git commands from drupal.org when switching
between issues? Me too.

To install, check the repo out somewhere and symlink /usr/local/bin/doop to doop
in the checkout.

NB: All these commands assume your clone of the repo is in a directory with the
same name as the repo.

## Switch issue:

```
doop <issue-number>
```

## Delete issue branch and remote. This won't do anything if the code isn't merged, like "git branch -d".

```
doop -d <issue-number>
```

## Force delete issue branch and remote. Like "git branch -D".

```
doop -D <issue-number>
```

## Push committed code to the right origin and branch.

```
doop push
```

This project is an experiment in (mostly) vibe coding with Claude Code.

## Verbose output

Use `-v` before any command to see the git commands being run. This is useful 
for seeing what's going wrong.

```
doop -v <issue-number>
doop -v push
```
