# Branch behind Workflow

This workflow is when the branch from where you created your working branch has been updated and
you need to update your working branch.

# Scenario

One of your teammates PR has been approved and merged to `preview`, now the branch from where you created the branch
you are currently working is an old version of `preview`, you need to update your local `preview` branch and your working branch. **REMEMBER**, none of your colleagues' changes affect your code. Ideally what you would do is:

1. Commit all your changes.

2. Run `git checkout preview` to switch to `preview`.

3. Run `git pull` to update preview.

4. Run `git checkout feature/your-branch` to switch back to your working branch.

5. Run `git rebase preview` to rebase with preview and update your working branch.

6. Run `git push -f origin feature/your-branch` to push your changes.

# Changes

# Preview

Change before rebasing with `preview`.

Change after rebasing with `preview`.
