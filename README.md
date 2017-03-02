# git-repo-update

bash script for git update multi folder

OPTIONS :

    -a : checkout & pull in spesific folder & branch
         example :
            to run command git checkout & pull for folder
            1. /html/code1 with branch master
            2. /html/code2 with branch develop
            
            usage :
            $ ./git-repo-update -a /html/code1:master,/html/code2:develop 

    -b : set branch name (default : master), this option use for option with -f & -p
    
    -p : set root path for multiple pull
    
    -f : set multiple folder to pull update (separate by comma)
    
    
EXAMPLE:

    - to pull multiple folder with one branch name
    
        example:
        pull folder /html/code1, /html/code2, /html/code3 with branch master
            
        usage :
        $ ./git-repo-update -p /html/ -f code1,code2,code3 -b master
        
    - to pull multiple folder with different branch name
    
        example :
        pull folder /html/code1 with branch master, pull folder /html/code2 with branch develop, pull folder /html/code3 with branch feature1
    
        usage :
        $ ./git-repo-update -a /html/code1:master,/html/code2:develop,/html/code3:feature1
        
