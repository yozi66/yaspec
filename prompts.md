gemini /specify Build an application that keeps track of my bonds, stocks and etfs and of my wife. There are multiple banks and accounts these assets are held at. There are special accounts called TBSZ to be opened for five years giving tax benefits if the assets are kept on these accounts without withdrawal.

gemini /plan
gemini /tasks
@specs/main/plan.md @specs/main/tasks.md @specs/main/data-model.md 

Modify the plan since we are about creating an electron project. It is not split to backend and frontend. 
Remove the backend and frontend dirs and look for an electron template with typescript, react and vite.

go on with the new plan

stop! xcopy has overwritten the current project's .git directory. Can we recover? 
Maybe checking out the current project to a temporary directory and copying back the .git directory? 
You can clone the current project from git@github.com:yozi66/yaspec.git

The many changes came from copying the electron-vite-react template onto the current project.
Please undo the changes and let's go back to the last commited state in git.

Apply the electron-vite-react template to the current project. 
It is tricky, since the standard way is to create a new project from the template. 
Please take care, we do not want to clone the electron-vite-react template onto our project (that was the problem last time). 

The standard way of using the template is npm create electron-vite@latest new-project-name 
It is an interactive prompt. Can you deal with it or is it better done by a human?

I did run the tool. The template was created as ../tmp-electron-vite-react-app  

Moved tmp-electron-vite-react-app into the current directory. You will be able to read it now.

Apply the electron-vite-react template to the current project. You can find it in tmp-electron-vite-react-app.

 @specs/main/plan.md @specs/main/tasks.md @specs/main/data-model.md
 adjust the plan and tasks to the current project structure
 