# Main Branch
- This branch will contain the stable and production-ready code.
- Only commits that have been reviewed and approved should be merged into this branch.

# Feature Branches
- **Naming convention**: `feat/this-is-feature-name`
- These branches will be used to develop **new features or enhancements.**
- Each feature branch should be **based on the main branch**.
- Only the developer working on the feature should merge the feature branch into the develop branch after completing the development and passing code review.

# Adding Features
Under no circumstances should you push to the main branch. Instead, follow these steps:
1. Create a new feature branch from the main branch.
2. Implement the feature or enhancement in the feature branch.
3. Write tests to cover the new feature or changes (also update docs if needed).
4. **Push your branch after rebasing the main branch:**
 	- Squash redundant commits before rebasing and pushing (e.g. WIP commits) ([Squash step-by-step](https://github.com/ittovate/.github/blob/main/docs/squash-steps.md))
 	- You must make sure that your PR will not result in merge conflicts.
	- If there are conflicts, you need to resolve them locally first.
5. **Create a pull request:** 
	- Write descriptive title.
	- Write changelog and reasons behind them.
	- Assign yourself for the task and assign reviewers.
	- Use **labels** to categorize PR and **milestones** to track progress.
6. **After approval:**
	1. Squash commits if needed, to remove redundant changes and make history easier to read.
	2. Merge the feature branch into the main branch.
	3. Delete remote branch.

# Commit Messages
- Commits should be **atomic** but it should include tests and docs for the same commit.
- Start the commit message with a **capital letter** and use the imperative mood (e.g., “Add feature” instead of “Added feature”).
- Use a clear, descriptive and concise but informative commit message (At most 72 characters but optimal is 50).
- **The commit message should explain why it was made:**
  - Tiny bit of ‘what’ but mostly focus on the ‘why’.
  - Reviewers must understand why it was made, and to be convinced that the change is good.
  - It's recommended to add body to commit message so that it's used in PR description.
- Reference relevant commmits.
- Reference relevant issues in the commit message using keywords like “Fixes,” “Closes,” or “Resolves” followed by the issue number (e.g., “Fixes #123”).
- Please avoid typos.

# FAQ
- What if the new task is dependent on open pull request?
	1. Work on that branch you need but without committing.
	2. If any changes were requested from reviewers on that PR:
		- **If it's your PR:** stash, modify & push, then apply stash.
		- **If it's NOT your PR:** when the changes are pushed, stash, pull, then apply stash.
	3. When PR is FINALLY merged:
		1. Stash the new task changes.
		2. Checkout to main and pull.
		3. Create a new branch for the new task and apply stash.
