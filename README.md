# Patches

This directory contains patches to be applied to the CORAL installation via the
`build.sh` script in the `scripts` directory.

Create patches on the command line using `git diff`. For example, if we are
creating a patch against the development branch use the following code template
from within the `web` directory:

```
git diff -w development my-branch > ../patches/development-##.my-branch.patch
```

The `-w` flag tells Git to ignore all whitespace changes. The `##` represents
two digits for applying patches in sequence.

If a patch is applicable to all branches, name it like:

```
all-##.my-patch-name.patch
```
