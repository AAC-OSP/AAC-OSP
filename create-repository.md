<h1> How to Push an Existing Project to GitHub Using VSC </h1>
<h2> Step 1 — Create a new GitHub Repo Using VSC </h2>
<p> Sign in to your Github account from vsc </p>
<img src="https://imgur.com/DpkhH2U.png" style="width:220px; height:100px">
<img src="https://imgur.com/Jd5Rpbr.png" style="width:420px; height:120px">
<p> Go to your Organizations </p>
<img src="https://imgur.com/9pISSBz.png" style="width:220px; height:500px">
<p> Click on AAC-Open-Source-Pool </p>
<img src="https://imgur.com/Tomrr6d.png" style="width:420px; height:100px">
<p> Click on New Repository </p>
<img src="https://imgur.com/MpzpYaV.png" style="width:220px; height:100px">
<p> Enter your project name</p>
<p> Set the repository to public and make sure to add the readme.md file </p>
<img src="https://imgur.com/qKoLNyf.png" style="width:420px; height:400px">
<p> Click on Create repository </p>
<img src="https://imgur.com/xWfmDAK.png" style="width:240px; height:150px">
<p> Click on Code and copy the link of the repository</p>
<img src="https://imgur.com/gysInUp.png" style="width:600px; height:400px">
<h2> Step 2 — Initialize Git in the project folder </h2>
<h3> git init </h3>
<p> This step creates a hidden .git directory in your project folder, which the git software admits and uses to store all the data and version history for the project.</p>
<h3> git add -A </h3>
<p> The git add command is used to tell git which files to include in a commit, and the -A (or --all) parameter means “include all”. </p>
<h3> git commit -m 'Added my project' </h3>
<p> The git commit command creates a new commit with all files that have been “added”. The -m (or --message) sets the message that will be included alongside the commit, used for future reference to understand the commit. In this case, the message is: 'Added my project'. </p>
<h3> git remote add origin git@github.com:<b> alexa007/your-project-name.git </b> </h3>
<h2> Note: Remember, you have to replace the bold parts of the username and repo name with your own username and repo name. </h2>
<p> In git, a “remote” refers to a remote version of the same repository. “origin” is the default name git gives to a remote server so git remote add origin is instructing git to add the URL of the default remote server for this repo. </p>
<h3> git push -u -f origin main </h3>
<p> The -u (or --set-upstream) flag sets the remote origin as the upstream reference. This allows you to later perform git push and git pull commands without having to specify an origin since we always want GitHub in this case.
The -f (or --force) flag stands for force. This will automatically overwrite everything in the remote directory. We’re using it here to overwrite the default README that GitHub automatically initialized.</p>
