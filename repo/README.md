# REPO COMMANDS

After going through this `README.md` file you will be familiar with all the `gh repo` commands.

## CREATE A REPO

Run the below command to open an interactive shell where you are asked for more details about the repo.

```md
gh repo create
```

Answer the questions prompted on the terminal

```md
% gh repo create

? What would you like to do? Create a new repository on GitHub from scratch
? Repository name hello (repo name)
? Repository owner akkshitgupta
? Description hello world
? Visibility Private/Public/Internal (select one)
? Would you like to add a README file? No
? Would you like to add a .gitignore? No
? Would you like to add a license? No
? This will create "hello" as a private repository on GitHub. Continue? (Y/n)
```

> Press Y to create the repo successfully

## COMMANDS for EXISTING REPO

1. shows the list of all the repos owned by you

   ```md
   gh repo list
   ```

2. fork a particular repo

   ```md
   gh repo fork [<owner/reponame>] # e.g, akkshitgupta/gh-cli
   ```

3. clone a repo to your `GitHub.com` account

   ```md
   gh repo clone [<owner/reponame>] # e.g, akkshitgupta/gh-cli
   ```

## Working with a Repo

1. view the repo `Description` and `README.md`

   ```md
   gh repo view # to view the current repo

   OR

   gh repo view [<owner/reponame>] # to view certain repo
   ```

   NOTE : Use `--web` flag at the end to open the repo in browser tab

2. List of all the `issues` corresponding to that repo

   ```md
   gh issue list
   ```

3. List of all the `Pull Requests` of that repo

   ```md
   gh pr list
   ```

4. Set a default repo for a local directory, in case of forked repo, for ease while dealing with `issue`, `PRs`, `GitHub Actions` , `releases`, and `secrets`

   ```md
   gh repo set-default
   ```

5. Create a **NEW** PR or issue using the following command

   ```md
   gh pr create

   <!-- or -->

   gh issue create
   ```
