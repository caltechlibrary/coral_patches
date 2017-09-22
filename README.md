# Patches

This directory contains patches to be applied to the CORAL installation via the
`build.sh` script in the `scripts` directory.

Create patches on the command line using `git diff`. For example, if we are
creating a patch against the development branch use the following code template
from within the `web` directory:

```
git diff -w development..my-branch > ../patches/my-branch.development.patch
```

The `-w` flag tells Git to ignore all whitespace changes.

_TODO:_ Create patches with a branch name in the filename to be applied to
different installations (production/master or test/development).
