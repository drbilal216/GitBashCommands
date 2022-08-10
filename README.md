# shift + insert 		to paste command in gitbash
# clear 			to clear all command

git config --global user.name DrBilal	# to set name
git config --global user.name		# to check name

git config --global user.email drbilal216@gmail.com	# to set email
git config --global user.name				# to see email

git init			# initialize repository
ls -lart			# show all hidden file folders
git status			# show files untrack, Unmodified, Modified Staged

git add GitBash-Code.txt	# staging area (add only 1 mentioned file)
git status			# now its shows file is staged and ready to commit
git commit			# open vim editter, press i and type your commit
				# then press esc, then type :wd to exit editor

touch abc.html			# touch command is use to create blank files

git add -A			# add all file to stagind area

git commit -m["Second commit"]	# better way to commit without vim editor

git checkout abc.html		# Restore selected file back to previous commit
				 (if something wrong is updated)
				 Very usefull command

git checkout -f			# Restore all file back to previous commit

git log				# show all commit
				# press q to quit
git log -p -3			# show 3 last commit also chow changes

git diff			# compare working tree with staging area
git diff -- staged		# compare staging area with last commit

git commit -a -m "Commit here"	# stage and commit (Not recomended for advance user)

ls 				# show all files of wurrent folder
touch waste.html		# create empty file name waste.html
git rm --cached waste.html	# remove from staging area not from directory
git rm waste.html		# remove from working directory and staging area of git

git status -s			# small status

touch .gitignore		# create file .gitignore

touch mylogs.log		# created file

# mylogs.log			# open .gitignore from notepad++
				# mention the file name you want to ignore
				# mylogs.log (ignore this file)
				# /mylogs.log (ignore this file in working folder not in child)
				# *mylogs.log (ignore all file name mylogs.log)
				# *.log (ignore all log file)
				# foldername/ (ignore this folder)

git branch feature1		# create a branch name feature1 (branch is a copy)
git branch			# show all available branches
git checkout feature1		# Switched to branch feature1
git checkout master		# Switched back to master branch
git merge feature1		# feature1 branch changes added to master branch
git checkout -b feature2	# Create a branch name feature2 and Switched to that branch

				# Create repositry in github
				# then connect to you local repository

git remote add origin https://github.com/drbilal216/GitBashCommands.git

git remote			# show all remote (origin)
git remote -v			# show url of fetch and push

git push origin master		# push local master to origin(Github)
git push -u origin master	# to push master branch
git push -u origin feature	# to push feature branch

git remote set-url origin https://github.com/drbilal216/GitBashCommands.git
				# if you want to change url

git clone https://github.com/drbilal216/GitBashCommands.git folderName
				# if you want to clone this repository
