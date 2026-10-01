Ans1) Using pwd printed '/Users/aaravbedi' which is my current working directory
Ans2) ls- a shows a few extra files starting with a '.' like '.config' and '.bash_profile'. The list of files also starts with a single dot on the first line followed by two dots on the second line.
Ans3) drwxr-xr-x    4 aaravbedi  staff    128 Jun 11 22:39 anaconda_projects
'drwxr-xr-x' refers to the file type and permissions. 'd' means its a directory. The next nine characters 'rwxr-xr-x' represent read/write/execute permissions for the owner, the group and everyone else respectively.
Ans4) It is a relative path
Ans5) The first time, mc moved the file 'README-backup.md' into the 'week01' folder, but kept its name the same. The second time, mv changed the file's name from 'README-backup.md' to 'old-readme.md' but it stayed in the same place. So basically, mv can either move a file, rename a file, or do both at once.
Ans6) 15
Ans7) /opt/anaconda3/bin/python3
Ans8) No, they're different. Mine is /opt/anaconda3/bin/python3 while theirs is /usr/bin/python3 . This is likely because I have Anaconda installed, which puts its own python3 in /opt/anaconda3/bin. My classmate probably doesn't have Anaconda installed, so their shell just used the regular Python that already came with their system instead.
Ans9) The shell said 'command not found'. That's because when I type a command, the shell checks every folder listed in my Path. Since pyton3 is a typo, there's no program with that name in any of the folders.
Ans10) .venv is a hidden folder starting with a dot and ls doesn't show hidden folders
Ans11) Once I activated the virtual environment, '.venv' showed up at the start of my prompt. That tells me the virtual environment is turned on, so now if I run python3 it uses the version inside .venv instead of the ones installed on my computer.
Ans12) No the path is not the same. After activating .venv it is '/Users/aaravbedi/Desktop/coding-cafe/.venv/bin/python3'. Activate adds the '.venv/bin' folder to the very front of my PATH. 
Ans13) The first list only had pip in it. After running pip install requests, the second list gained five new packages: 'requests' itself, 'certifi', 'charset-normalizer', 'idna' and 'urllib3'.
Ans14) /opt/anaconda3/bin/python3
Ans15) Instead of showing file sizes as big raw number of bytes, it shows them in KB, MB or GB making them way easier to understand.
Ans16) Ctrl+C forcibly stops whatever program is currently running and shows 'KeyboardInterrupt'. Ctrl+D sends an End of line signal which tells a program that there's no more input and that it can end on its own instead of being killed.