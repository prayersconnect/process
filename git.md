## Git Workflow

### Starting a new branch
- Checkout `main`
- Pull latest `main` from `remote` (`git pull`)
- Create new branch (`git checkout -b <FEATURE_BRANCH>`)
- _Commit as needed_
- Push branch `git push origin <FEATURE_BRANCH>`

### Review Process
1. Once code is pushed, create a Pull Request (PR) against `staging` branch. 
1. Get the PR reviewed, approved & merged. Reviewers should review PR based on A/C criteria of the ticket.
1. Once merged to `staging`, wait for deployment, verify staging environment (by implementer, reviewer etc.). Review [Definition of Done](https://github.com/prayersconnect/process/blob/main/agile.md#definition-of-done) for details
1. Once everything is verified, recreate the PR against `main` branch. 
1. Follow same process mentioned in step 2 & 3 but for `main` branch (production environment).
1. Verify production environment by all parties involved. 
1. Close ticket.
