- check git version:`git --version`
- install git:`brew install git`
  - if `xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun`: run `xcode-select --install`
- If the Command Line Tools are already installed, you can try resetting the path by running the command `xcode-select --reset`
 ## Set up SSH with Github
 - follow this:https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
 - DON'T CHANGE THE KEY NAME! DEFAULT NAME IS:id_ed25519
 - the default path of the key is:`/Users/YOUR_NAME/.ssh/id_ed25519`, if no such file: `mkdir -p ~/.ssh`
 - if `Permissions 0777 for '/Users/YOUR_NAME/.ssh/id_ed25519' are too open.
It is required that your private key files are NOT accessible by others.
This private key will be ignored.` , run `chmod 600 ~/.ssh/id_ed25519`
 - check if key existed:`ls |grep id_ed25519`, then run `cat id_ed25519.pub` to see and copy the public key
