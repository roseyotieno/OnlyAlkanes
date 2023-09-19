# Commands used to push only the .pdb files whose number suffix is divisible by 10
---

- git clone git@github.com:roseyotieno/OnlyAlkanes.git
- cp -a alkanes/ OnlyAlkanes/
- for j in `ls *.pdb`; do for k in {1..100}; do cp $ j $(basename -s .pdb $j)$k.pdb; done; 
- git add *0.pdb
- git status
- git commit -m "push only the .pdb files whose number suffix is divisible by 10"
- git push
- git status
