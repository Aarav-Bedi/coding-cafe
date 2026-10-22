# Lab 4: Git & GitHub Notes

## Question 1
--global means the setting is saved for my whole computer (in ~/.gitconfig), so every repo I make uses the same name and email. Without it, the setting would only apply to the one repo I'm in, and the command wouldn't even work outside a repo.

## Question 2
The hidden `.git` directory appeared in `ls -a` but not in `ls`, because names starting with a dot are hidden. It stores Git's information about the repository, including its settings and commit history.

## Question 3
Git offered to track about 1065 files and folders, which was mostly the contents of `.venv/`. The `.venv/` entries are not something I wrote, since they are other people's installed packages, and `.DS_Store` is macOS clutter, so none of that belongs in the repository.

## Question 4
The `.venv/` folder and `.DS_Store` disappeared from `git status`. Only my own work is left (`.gitignore`, `README.md`, and the week folders), because the ignore rules tell Git to skip those entries.

## Question 
I should commit .gitignore because it contains the rules for which files Git should ignore. Keeping it in the repository means those rules are shared with anyone else working on the project.

## Question 6
`README.md` moved from "Untracked files" to "Changes to be committed". In the three-places model, it moved from the working directory to the staging area, which means it is ready to go into the next commit but is not saved in history yet.

## Question 7
After the commit, Git printed [main (root-commit) 5d75c82] Lab work so far and said 4 files changed, with 37 insertions. The files were .gitignore, README.md, week02/lab01-log.txt and week02/notes.md. "root-commit" means it was the first commit in the repo.

## Question 8
The first seven characters are the short commit hash (for example `a1b2c3d`), which is the beginning of the commit's full 40-character ID. It is used to refer to one specific commit, for example when looking at it or going back to it, and it is short enough to type.

## Question 9
The loop is: (1) edit or create files, (2) check what changed with `git status`, (3) stage the changes with `git add`, and (4) save them with `git commit`. `git log --oneline` can then be used to confirm the new commit is in the history.

## Question 10
`README.md` has a special name and place because it is a convention: it sits in the root of the repository so it is the first thing a reader sees. GitHub also looks for that exact filename and displays it on the repository's front page, so it works as the project's introduction.

## Question 11
`gh auth login` signed me in to GitHub through the browser and saved an access token on my computer. Because I chose to authenticate Git, Git now uses that saved token whenever I push over HTTPS, so it does not need to ask for a password.

## Question 12
The front page shows the contents of my `README.md`, rendered as formatted text, with the list of files below it. GitHub shows it because it automatically displays the README in the root of a repository as the project's front page.

## Question 13
No, pushing did not change my local history. `git log --oneline` shows the same commits as before, because a push only copies my local commits to GitHub. The only difference is that Git now also tracks where the remote (`origin/main`) is.

## Question 14
A private repository does exist on GitHub, with all my files and history stored there, but only I and the people I invite (like the TAs) can see it. A repository that does not exist on GitHub has no online copy at all, so there is nothing for anyone to access and no cloud backup.