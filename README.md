 

 # Different Features of Git Commit with Explanations and Examples

## 1. **Message Description**
Every commit has a message that describes the changes made. Commit messages help you and your team understand the purpose of each change.

### Example:
```sh
git commit -m "Refactored login feature for better performance"
git commit -m "feat: add dark mode toggle in user settings"
git commit -m "fix: resolve issue with form validation not triggering on submit"
git commit -m "docs: update API usage examples in README"
git commit -m "style: fix indentation and remove trailing spaces in main.css"
git commit -m "refactor: rename 'userData' to 'userProfile' for better clarity"
git commit -m "test: add unit tests for authentication middleware"
git commit -m "chore: update eslint config to enforce new style rules"

## 2. **Amend Previous Commit**  
Modify the most recent commit to fix mistakes or add missing files.

### Example:
```sh
git commit --amend -m "Optimize search algorithm for better performance"
git commit --amend -m "fix: update error message for better clarity"


## 3. **Staging Partial Changes**  
Commit only selected changes from a file.

### Example:
```sh
git add -p
git commit -m "Update footer content for improved branding"

git add -p  
git commit -m "fix: correct tax calculation logic in checkout process"

## 4. **Sign-Off (Verified Commits)**  
Certify your commits with a sign-off.

### Example:
```sh
git commit -s -m "Refactored authentication module for efficiency"
git commit -s -m "feat: add email verification step in user registration"
git commit -s -m "fix(security): enforce strong password policies"


## 5. **Committing with Author Identity**  
Specify a different author for a commit.

### Example:
```sh
git commit --author="Michael Doe <michael.doe@example.com>" -m "Improve error logging"
git commit --author="Sarah Lee <sarah.lee@example.com>" -m "fix: adjust timezone conversion in reports"

## 6. **Empty Commits**  
Create a commit without changing files, useful for triggering workflows.

### Example:
```sh
git commit --allow-empty -m "Triggering CI build"
git commit --allow-empty -m "chore(ci): force rebuild after config changes"

## 7. **Squashing Commits**  
Merge multiple commits into one for a cleaner history.

### Example:
```sh
git rebase -i HEAD~3
git rebase -i HEAD~5  # Mark unwanted commits as "squash" (s)

## 8. **Interactive Rebase**  
Modify, reorder, or delete past commits.

### Example:
```sh
git rebase -i HEAD~4
git rebase -i HEAD~6

## 9. **Diff Viewing Before Commit**  
Preview changes before committing.

### Example:
```sh
git diff --staged
git add -p  
git commit -m "fix: correct pricing logic in discount calculation"

## 10. **GPG-Signed Commits**  
Sign commits with a GPG key for authentication.

### Example:
```sh
git commit -S -m "Enhance API security with rate limiting"
git commit -s -m "feat: add webhook support for third-party integrations"