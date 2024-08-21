# Branch conflicts with preview

This workflow is when you are making changes but one of your colleagues changes where approved and merged before yours theres conflicts betwen the changes.

To showcase a better real-life scenario I added [Astro](https://astro.build/) as the project's framework.

The example is really simple. Say your making a Blog Web App. Your working on the pagination of the page whereas your colleague is working on the layout of the page. If your colleague changes where approved and merged before yours and he made changes that affect your code (hypothetically you are not aware of this), then when you merge your branch with the `preview` branch there will be conflicts you will have to deal with.

Normally what you will want to do is:

1. Commit your changes.
2. If your branch is not published use `git rebase preview` if not, run `git merge colleague-branch` to merge your branch with your colleague branch.
3. Resolve the conflicts.
