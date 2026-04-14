
		`			ps-1
🔹 Initialize repo
mkdir ds_project
cd ds_project
git init
________________________________________
🔹 Connect to GitHub
git remote add origin https://github.com/YOUR-USERNAME/ds_project.git
________________________________________
🔹 Create program1
touch program1.py
________________________________________
🔹 Add, commit, push (main branch)
git add .
git commit -m "Added program1"
git branch -M main
git push -u origin main
________________________________________
🔹 Create new branch
git checkout -b GIT-EXAM
________________________________________
🔹 Create program2
touch program2.py
________________________________________
🔹 Add, commit, push (GIT-EXAM)
git add .
git commit -m "Added program2"
git push -u origin GIT-EXAM
________________________________________
🔹 Show difference between branches
git diff main GIT-EXAM
________________________________________
🔹 (Optional) Check branch
git branch


		ps-3
mkdir ds_project
cd ds_project
git init
________________________________________
🔹 b. Connect to GitHub
git remote add origin https://github.com/YOUR-USERNAME/ds_project.git
________________________________________
🔹 c. Create branch GIT-EXAM-1 + program2 (palindrome)
git checkout -b GIT-EXAM-1
touch program2.py
________________________________________
🔹 d. Create program1 (squares)
touch program1.py
________________________________________
🔹 e. Add, commit, push
git add .
git commit -m "Added program1 and program2 in GIT-EXAM-1"
git push -u origin GIT-EXAM-1
________________________________________
🔹 f. Create new branch GIT-EXAM-2
git checkout -b GIT-EXAM-2
________________________________________
🔹 g. Pull changes from GIT-EXAM-1
git pull origin GIT-EXAM-1
________________________________________
🔹 h. Create program2 again (or modify)
touch program2.py
________________________________________
🔹 i. Modify program1 (to create conflict)
# open program1.py and change logic
________________________________________
🔹 j. Commit and push
git add .
git commit -m "Modified program1 and program2 in GIT-EXAM-2"
git push -u origin GIT-EXAM-2
________________________________________
🔹 Show differences between branches
git diff GIT-EXAM-1 GIT-EXAM-2
git diff main GIT-EXAM-1
git diff main GIT-EXAM-2
________________________________________
🔹 k. Create Pull Request (GIT-EXAM-2 → GIT-EXAM-1)
git push origin GIT-EXAM-2



                                      PS-4

🔹 a. Initialize repository
mkdir ds_project
cd ds_project
git init
________________________________________
🔹 b. Connect to GitHub
git remote add origin https://github.com/YOUR-USERNAME/ds_project.git
________________________________________
🔹 c. Create branch + program2 (palindrome)
git checkout -b GIT-EXAM-1
touch program2.py
👉 Write code in program2.py:
string = input("Enter a string: ")
if string == string[::-1]:
    print("Palindrome")
else:
    print("Not Palindrome")
________________________________________
🔹 d. Create program1 (squares)
touch program1.py
👉 Write code:
for i in range(1, 11):
    print(i*i)
________________________________________
🔹 e. Commit and push
git add .
git commit -m "Added program1 and program2"
git push -u origin GIT-EXAM-1
👉 Check on GitHub → both files visible ✅
________________________________________
🔹 f. Create IGNORE directory and files
mkdir IGNORE
cd IGNORE
touch test1.txt test2.txt
cd ..
________________________________________
🔹 g. Create .gitignore and ignore folder
touch .gitignore
👉 Open .gitignore and write:
IGNORE/
________________________________________
🔹 h. Commit and push
git add .
git commit -m "Added gitignore to ignore IGNORE folder"
git push
________________________________________
🔍 How to prove IGNORE folder is NOT pushed
Check status:
git status
👉 You will NOT see:
IGNORE/test1.txt
IGNORE/test2.txt
________________________________________
Check on GitHub:
•	Open repo on GitHub 
•	You will see: 
o	✅ program1.py 
o	✅ program2.py 
o	❌ IGNORE folder NOT present


                                   PS-5
a. Initialize repository
1.	Open GitHub Desktop 
2.	Click File → New Repository 
3.	Fill: 
o	Name: ds_project 
o	Local path: choose folder 
4.	Click Create Repository 
________________________________________
🔹 b. Publish to GitHub
1.	Click Publish repository 
2.	Choose: 
o	Account (your GitHub) 
o	Keep repo Public/Private 
3.	Click Publish Repository 
👉 Now repo is on GitHub
________________________________________
🔹 c. Create branch + program2
1.	Click Current Branch → New Branch 
2.	Name: GIT-EXAM-1 
3.	Click Create Branch 
👉 Now create file:
•	Go to project folder 
•	Create program2.py 
Add code:
string = input("Enter a string: ")
if string == string[::-1]:
    print("Palindrome")
else:
    print("Not Palindrome")
________________________________________
🔹 d. Create program1
•	Create file program1.py 
Add code:
for i in range(1, 11):
    print(i*i)
________________________________________
🔹 e. Commit and push
1.	Go to GitHub Desktop 
2.	You will see changes listed 
3.	Add message:
👉 Added program1 and program2 
4.	Click Commit to GIT-EXAM-1 
5.	Click Push origin 
👉 Check on GitHub → files visible ✅
________________________________________
🔹 f. Create IGNORE folder
1.	In project folder: 
o	Create folder: IGNORE 
o	Inside create: 
	test1.txt 
	test2.txt 
________________________________________
🔹 g. Create .gitignore
1.	In project folder create file:
👉 .gitignore 
2.	Add this line: 
IGNORE/
________________________________________
🔹 h. Commit and push
1.	Open GitHub Desktop 
2.	You will see .gitignore change 
3.	Add message:
👉 Added gitignore to ignore IGNORE folder 
4.	Click Commit 
5.	Click Push origin 
________________________________________
🔍 Verify (Important)
In GitHub Desktop:
•	You will NOT see test1.txt, test2.txt 
On GitHub:
You will see:
program1.py
program2.py
.gitignore
❌ You will NOT see:
IGNORE/
test1.txt
test2.txt
________________________________________
⚠️ If IGNORE folder appears (common mistake)
In GitHub Desktop:
1.	Right-click IGNORE folder 
2.	Remove from repository (keep local) 
3.	Commit again 
4.	Push 
________________________________________
🎯 Viva Answer
👉 “GitHub Desktop provides a GUI to manage repositories. .gitignore is used to prevent files from being tracked and pushed.”
________________________________________
If you want, I can give you a quick comparison (Git Bash vs GitHub Desktop) for exam 👍


                                            PS-6

USING GIT DESKTOP
Here’s the step-by-step solution using GitHub Desktop (GUI) 👇
________________________________________
🔹 a. Clone repository
1.	Open GitHub Desktop 
2.	Click File → Clone Repository 
3.	Select URL tab 
4.	Paste:
https://github.com/KalyanM45/AI-Project-Gallery.git
5.	Click Clone 
________________________________________
🔹 b. Show branch creation is disallowed
1.	Click Current Branch → New Branch 
2.	Name: test-branch 
3.	Click Create Branch 
4.	Click Push origin 
👉 ❌ You will get error (permission denied)
👉 This proves you cannot push to original repo
________________________________________
🔹 c. Fork repository
1.	Go to GitHub 
2.	Open the repo 
3.	Click Fork 
________________________________________
🔹 d. Clone YOUR fork
1.	In GitHub Desktop → File → Clone Repository 
2.	Choose your forked repo (YOUR-USERNAME/AI-Project-Gallery) 
3.	Click Clone 
________________________________________
🔹 e. Create feature branch
1.	Click Current Branch 
2.	Click New Branch 
3.	Name: GIT-EXAM 
4.	Click Create Branch 
________________________________________
🔹 f. Make changes
1.	Open project folder 
2.	Create a new file: 
o	my_changes.py 
3.	Add any code and save 
________________________________________
🔹 g. Commit and push
1.	Go back to GitHub Desktop 
2.	You will see changes 
3.	Add message:
👉 Added new feature 
4.	Click Commit to GIT-EXAM 
5.	Click Push origin 
________________________________________
🔹 h. Create Pull Request
1.	Click Create Pull Request (in GitHub Desktop) 
2.	Browser opens on GitHub 
3.	Click Create Pull Request 
________________________________________
🔹 i. Resolve merge conflicts (if any)
👉 If conflict shown:
1.	GitHub Desktop will show conflict warning 
2.	Click Open in editor 
3.	You’ll see:
<<<<<<< HEAD
your code
=======
other code
>>>>>>> main
4.	Edit and fix 
5.	Save file 
Then:
•	Click Mark as resolved 
•	Commit 
•	Push 
________________________________________
🔹 j. Incorporate feedback
1.	Make changes in files 
2.	In GitHub Desktop: 
o	Commit changes 
o	Push 
👉 Pull Request updates automatically ✅
________________________________________
🎯 Final Flow
Clone → Fail push → Fork → Clone fork → Branch → Change → Commit → Push → PR → Resolve conflicts
________________________________________
🧠 Viva Answer
👉 “Using GitHub Desktop, we fork the repository, create a branch, commit changes, and create a pull request to contribute to the original repository.”




     USING GITBASH
Got it — here is the complete solution using ONLY Git Bash (with minimal GitHub UI where required) 👇
________________________________________
🔹 a. Clone repository
git clone https://github.com/KalyanM45/AI-Project-Gallery.git
cd AI-Project-Gallery
________________________________________
🔹 b. Show branch creation/push is disallowed
git checkout -b test-branch
git push origin test-branch
👉 You will get error (permission denied)
👉 This proves you cannot push to original repo
________________________________________
🔹 c. Fork the repository (ONE UI step needed)
👉 Go to GitHub
👉 Click Fork
________________________________________
🔹 d. Connect your fork using Git Bash
git remote rename origin upstream
git remote add origin https://github.com/YOUR-USERNAME/AI-Project-Gallery.git
👉 Now:
•	upstream = original repo 
•	origin = your fork 
________________________________________
🔹 e. Push code to your fork
git push -u origin main
________________________________________
🔹 f. Create feature branch
git checkout -b GIT-EXAM
________________________________________
🔹 g. Make changes
touch my_changes.py
(Add any code inside file)
________________________________________
🔹 h. Commit and push
git add .
git commit -m "Added new feature"
git push -u origin GIT-EXAM
________________________________________
🔹 i. Create Pull Request (via Git Bash link)
git request-pull upstream/main origin GIT-EXAM
👉 Copy the generated link and open in browser
👉 Click Create Pull Request
________________________________________
🔹 j. Resolve conflicts (if any)
git fetch upstream
git merge upstream/main
👉 Fix conflict manually → then:
git add .
git commit -m "Resolved conflicts"
git push
________________________________________
🔹 k. Update after feedback
git add .
git commit -m "Updated as per review"
git push
________________________________________
🎯 Final Concept
•	Clone → no permission to push 
•	Fork → your copy 
•	Branch → make changes 
•	Push → your fork 
•	PR → send changes to original repo 
________________________________________
🧠 Viva Answer
👉 “Using Git Bash, we fork the repository, create a feature branch, push changes to our fork, and create a pull request to contribute to the original repository.”
________________________________________
If you want, I can give you a super short exam version (just commands in 10 lines) 👍
USING GIT DESKTOP
Here’s the step-by-step solution using GitHub Desktop (GUI) 👇
________________________________________
🔹 a. Clone repository
1.	Open GitHub Desktop 
2.	Click File → Clone Repository 
3.	Select URL tab 
4.	Paste:
https://github.com/KalyanM45/AI-Project-Gallery.git
5.	Click Clone 
________________________________________
🔹 b. Show branch creation is disallowed
1.	Click Current Branch → New Branch 
2.	Name: test-branch 
3.	Click Create Branch 
4.	Click Push origin 
👉 ❌ You will get error (permission denied)
👉 This proves you cannot push to original repo
________________________________________
🔹 c. Fork repository
1.	Go to GitHub 
2.	Open the repo 
3.	Click Fork 
________________________________________
🔹 d. Clone YOUR fork
1.	In GitHub Desktop → File → Clone Repository 
2.	Choose your forked repo (YOUR-USERNAME/AI-Project-Gallery) 
3.	Click Clone 
________________________________________
🔹 e. Create feature branch
1.	Click Current Branch 
2.	Click New Branch 
3.	Name: GIT-EXAM 
4.	Click Create Branch 
________________________________________
🔹 f. Make changes
1.	Open project folder 
2.	Create a new file: 
o	my_changes.py 
3.	Add any code and save 
________________________________________
🔹 g. Commit and push
1.	Go back to GitHub Desktop 
2.	You will see changes 
3.	Add message:
👉 Added new feature 
4.	Click Commit to GIT-EXAM 
5.	Click Push origin 
________________________________________
🔹 h. Create Pull Request
1.	Click Create Pull Request (in GitHub Desktop) 
2.	Browser opens on GitHub 
3.	Click Create Pull Request 
________________________________________
🔹 i. Resolve merge conflicts (if any)
👉 If conflict shown:
1.	GitHub Desktop will show conflict warning 
2.	Click Open in editor 
3.	You’ll see:
<<<<<<< HEAD
your code
=======
other code
>>>>>>> main
4.	Edit and fix 
5.	Save file 
Then:
•	Click Mark as resolved 
•	Commit 
•	Push 
________________________________________
🔹 j. Incorporate feedback
1.	Make changes in files 
2.	In GitHub Desktop: 
o	Commit changes 
o	Push 
👉 Pull Request updates automatically ✅
________________________________________
🎯 Final Flow
Clone → Fail push → Fork → Clone fork → Branch → Change → Commit → Push → PR → Resolve conflicts
________________________________________
🧠 Viva Answer
👉 “Using GitHub Desktop, we fork the repository, create a branch, commit changes, and create a pull request to contribute to the original repository.”
________________________________________
If you want, I can give you a short 5-step version for writing in exam 👍







