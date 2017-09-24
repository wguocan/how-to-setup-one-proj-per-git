1.	Create a git repo at remote server

	e.g, create a new git repotory named how-to-setup-openssh

	or, at a git server:
 
		mkdir how-to-setup-openssh

		cd how-to-setup-openssh

		git init --bare

2. Create a project at local machine

	mkdir ~/some-git-projects/how-to-setup-openssh

	cd ~/some-git-projects/how-to-setup-openssh

	git init

	vi README.md

3. Commit the project to local repository

	git add .

	git commit -m 'Initial commit'

4. Setup remote repository and push the project to remote

	git remote add origin https://CWBitbucket@bitbucket.org/CWBitbucket/how-to-setup-openssh

	git push -u origin master

	or change remote git url: git remote set-url origin https://CWBitbucket@bitbucket.org/CWBitbucket/how-to-setup-openssh
	
5. Verify to clone the project from remote repository

	At local machine:

	mkdir /tmp/verify-project

	cd /tmp/verify-project

	git clone https://CWBitbucket@bitbucket.org/CWBitbucket/how-to-setup-openssh.git . (use dot)
