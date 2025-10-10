1. 

Someone creates the project repo (on GitHub, for example), then everyone else **clones** it:

	git clone https://github.com/teamname/project.git

That gives you a full copy of the project with all its history.

2. 

Do your edits, add your code, fix bugs — whatever your task is.

3. 

check what you changed

	git status

You'll see which files are new or modified. 

4. 

add your changes to the next "save point"

	git add .
	git commit -m "added the new login form"

The -m is to add a message written in " ". this is mandatory.
when typing these commands it saves your snapshot locally. 

5. 

Now push tour changes 

	git push 

this uploads your work to the shared github repository so everyone else can see it. 

6. 

before you start working (and before pushing new changes) always do

	git pull

That gets teh newest versison of the project - so you dont overwrite anyones work. 