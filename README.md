1.	Create a git repository at remote server

	e.g, create a new git repository named how-to-setup-one-proj-per-git

	or, at a git server:
 
		mkdir how-to-setup-one-proj-per-git

		cd how-to-setup-one-proj-per-git

		git init --bare

2. Create a project at local machine

	mkdir ~/some-git-projects/how-to-setup-one-proj-per-git

	cd ~/some-git-projects/how-to-setup-one-proj-per-git

	git init

	vi README.md

3. Commit the project to local repository

	git add .

	git commit -m 'Initial commit'

4. Setup remote repository and push the project to remote

	git remote add origin https://github.com/wguocan/how-to-setup-one-proj-per-git.git

	git push -u origin master

	or change remote git url: git remote set-url origin https://github.com/wguocan/how-to-setup-one-proj-per-git.git
	
5. Verify to clone the project from remote repository

	At local machine:

	mkdir /tmp/verify-project

	cd /tmp/verify-project

	git clone https://github.com/wguocan/how-to-setup-one-proj-per-git.git . (use dot to avoid creating additional folder)
