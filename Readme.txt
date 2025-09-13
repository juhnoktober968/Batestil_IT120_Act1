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
