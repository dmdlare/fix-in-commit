Using "fix" in GitHub Commits

When making a commit that fixes an issue, it's important to write a clear and descriptive commit message. Below are different examples of how "fix" can be used in commit messages:

1. Bug Fixes

fix: resolve crash when clicking on profile button

fix(login): correct wrong password validation

fix: prevent null pointer exception in user service

fix(api): handle timeout errors properly


2. UI/UX Fixes

fix(ui): align buttons properly in mobile view

fix(css): make navbar responsive on smaller screens

fix: dark mode colors for better contrast


3. Code Improvements

fix: remove unused variables causing warnings

fix(memory-leak): properly dispose event listeners

fix(performance): optimize database query execution


4. Documentation Fixes

fix(docs): update installation guide with correct commands

fix(readme): correct typo in project setup steps


Example Use Case

Scenario:

You're working on a web app, and a user reports that clicking the "Submit" button multiple times sends duplicate form entries.

After debugging, you find that the issue is caused by the button not being disabled after the first click. You fix it by adding a disabled attribute to prevent multiple submissions.

Commit Example:

fix(form): prevent duplicate submissions by disabling button

Previously, users could submit the form multiple times by clicking the submit button repeatedly.  
This fix disables the button on the first click and prevents duplicate entries.

This message clearly explains:
What was fixed
Why it was a problem
How it was fixed
