mkdir Batestil_IT120_Act1
cd Batestil_IT120_Act1
git init 
touch Profile.txt Education.txt Background.txt Readme.txt Test.py
git add .
git commit -m "Initial commit"
git branch Batestil_B1
git branch Batestil_B2
git branch Batestil_B3
git branch Batestil_B4
git checkout Batestil_B1
git add Profile.txt Readme.txt
git commit -m "Amend Profile.txt to Batestil_B1, also add command in Readme.txt"
git checkout Batestil_B2
git add Education.txt Readme.txt
git commit -m "Amend Education.txt to Batestil_B2, also add command in Readme.txt"
git checkout Batestil_B2
git add Education.txt Readme.txt
git commit -m "Amend Education.txt to Batestil_B2, also add command in Readme.txt"
git checkout Batestil_B3
rm Test.py
git add Background.txt Test.py
git commit -m "Amend Background.txt & remove Test.py to Batestil_B3, also add command in Readme.txt"
git checkout Batestil_B4
rm Test.py
git add Test.py Readme.txt
git commit -m "Amend in Readme.txt and remove Test.py"
git checkout master
git remote add origin https://github.com/juhnoktober968/Batestil_IT120_Act1.git
git push origin --all
git merge Batestil_B1
git merge Batestil_B2
git commit -m "merge education and readme from branch Batestil_B2"
git merge Batestil_B3
git commit -m "merge background and readme from branch Batestil_B3"
git merge Batestil_B4
git commit -m "merge readme excluding Test.py from Batestil_B4"