rmcat-eval-criteria
====================

use `make deploy` to build a specific version of the document.
the command line utility asks which version, choose 00 (for initial document)
or appropriate number when asked.

```bash
$ make deploy
version: 00
```

On submission of a draft to the datatracker, please tag it. In that way we just maintain one xml version and the -xx versions stay static. Command to tag a commit version is:

```bash
$ git tag -a draft-name -m "version xx for individual/IETF submission"
$ git push --tags
```

If you made a mistake with the tag naming, a new tag can replace by follow the instructions on [Stack Overflow](http://stackoverflow.com/questions/1028649/rename-a-tag-in-git):

```bash
git tag new-tag old-tag
git tag -d old-tag
git push origin :refs/tags/old-tag
git push --tags
```
==================
