# Contributing
 
Issues and pull requests are welcome.
 
## Getting access
 
New contributors need to be verified before they can contribute:
1. Send your GitHub account link to An0n on Threema: [Contact An0n on Threema](https://threema.id/87YD3CY3)
2. An0n adds you to the contributor team of this repository in the `sprac-ch` organisation.

This is a security measure. It prevents people from impersonating SPARC Community members.

> [!WARNING]
> Use a burner account for opsec reasons.
>
> Questions about SPARC should not be discussed here (as in not on GitHub, or any public forum for that matter).
> Please contact either [SPARC directly](https://sparc-cyberdefence.ch/us/contact/) or, if community-related, [An0n](https://threema.id/87YD3CY3).
 
## Workflow

As a contributor you have write access to this repository, so there is no need to fork it. Work on a branch and never push directly to `main`.

1. Clone the repository:
   ```bash
   git clone https://github.com/sprac-ch/resources.git
   cd resources
   ```
2. Make sure your commit identity does not leak personal data. Use your burner account details, for example the GitHub noreply address:
   ```bash
   git config user.name "your-burner-username"
   git config user.email "your-burner-username@users.noreply.github.com"
   ```
3. Create a feature branch from an up-to-date `main`:
   ```bash
   git switch main
   git pull
   git switch -c feat/short-description
   ```
4. Add your file (only SVG format is accepted) in the matching directory and follow the naming convention in the [README](README.md#naming-convention).
5. Commit using [Conventional Commits](https://www.conventionalcommits.org/) style messages, for example `chore: add custom pfp of student`:
   ```bash
   git add .
   git commit -m "chore: add custom pfp of student"
   ```
6. Push your branch to the repository:
   ```bash
   git push -u origin feat/short-description
   ```
7. Open a pull request from your branch into `main` and wait for review. If changes are requested, push further commits to the same branch.

For suggestions, use the [issue tracker](https://github.com/sprac-ch/resources/issues).
