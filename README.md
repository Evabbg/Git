useful tutorial: https://www.youtube.com/watch?v=RGOj5yH7evk
## Set up SSH with Github
 - follow this: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
 - DON'T CHANGE THE KEY NAME! DEFAULT NAME IS:id_ed25519.
 - the default path of the key is:`/Users/YOUR_NAME/.ssh/id_ed25519`, if no such file: `mkdir -p ~/.ssh`.
 - if `Permissions 0777 for '/Users/YOUR_NAME/.ssh/id_ed25519' are too open.
It is required that your private key files are NOT accessible by others.
This private key will be ignored.` , run `chmod 600 ~/.ssh/id_ed25519`.
 - copy the public key: first go the the diretory where the key is in: `cd ~/.ssh/`, then run `cat id_ed25519.pub` to see and copy the public key.

## Download git
- check git version:`git --version`
- install git:`brew install git`
  - if `xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun`: run `xcode-select --install`
- If the Command Line Tools are already installed, you can try resetting the path by running the command `xcode-select --reset`

## Git commands
- `git init`: Initializes a new Git repository in the current directory.
- `git clone`: Clones an existing Git repository into a new directory.
- `git status`: Shows the status of the current working directory and any changes that have been made.
- `git add`: Adds changes to the staging area in preparation for committing them to the repository.
    - `git add .` : add all the changes
    - `git add README.md` : only add changes in README.md
- `git commit -m "test" -m "test"`: Commits changes to the repository, creating a new snapshot of the project's state. m describes this commit.
- `git push origin main`: Pushes committed changes in 'main' branch to a remote repository, typically hosted on a service like GitHub or Bitbucket.
- `git pull`: Pulls changes from a remote repository and merges them into the current branch.
- `git branch`: Lists all local branches in the repository.
    - `git branch test`: create a new branch call "test".
- `git checkout`: Switches to a different branch or commit.
    -`git checkout test`: swicth to 'test' branch.
- `git merge`: Merges changes from one branch into another.
- `git log`: Shows a history of all commits in the repository.




