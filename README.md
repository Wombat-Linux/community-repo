
The Community Package Repository
==========
Welcome to the Wombat Linux community package repository.

## How to submit to the community package repository

1. Create a fork of the repository
2. Add your chosen package file
3. Modify the `packages.json` file with the name and MD5 hash of your package. For an example: 
```json
{
	...
	"mypackage":"da49bdf9405dd9a6e44808bfe9e6dfcf"
	...
}
```
4. Create a pull request with a general description of the package (AKA what it does or its uses) and thats about it.
5. Done!

## Rules

(based on the [AUR submission guidelines](https://wiki.archlinux.org/index.php/AUR_submission_guidelines))

When submitting a package to the community repository, observe the following rules:

-   The submitted .uspm(s) must not build applications  **already in any**  of the  **official**  binary  **repositories**  under any circumstances. Check the  [official package database](https://packages.afroraydude.com/wombatlinux/uspm)  for the package. If the most up-to-date version of it exists,  **do not**  submit the package. If the official package is out-of-date, you may create a pull request with that information within the request.

-   **Check the Community Package Repository**  if the package  **already exists**. If it is currently maintained, changes can be submitted in a comment for the maintainer's attention. If it is unmaintained or the maintainer is unresponsive, the package can be adopted and updated as required, and you may do as above.

The community package repository and official repositories are intended for packages which install generally software and software-related content, including one or more of the following: executables, libraries, configuration setups, etc.

-   If a package needs to be fixed due to some incompatibility **IN AND ONLY IN** either the `PACKAGECODE` or the `PACKAGEDATA` files, create a pull request.

-   Packages that **do not** use  prebuilt  [deliverables](https://en.wikipedia.org/wiki/Deliverable), when the prebuilt package is available, must have `-src` appended to the package name (ie: `uspm-main-src`). 
