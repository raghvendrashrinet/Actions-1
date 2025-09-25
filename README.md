# Exploring GitHub Actions
 We will be learnig GitHub Action Daily and make and progress entry heare

 ## Day-1 25092015 
  1. Accessed github.dev for vscode editor
  2. Installed Github Actions Extenshions for vscode 
  3. Create folder .github/workflows, which will have workflow yaml files
  4. Create first workflow : workflow-ex-1
  
## working on the workflow file
 use ctrl+ tab to get auto suggestion

<pre>
 name: First workflow  
 on: push  
 jobs:  
    first_job:  
       runs-on: ubuntu-latest   
         steps:  
            - name : checkout
              uses : actions/checkout@v4

            - name : welcome message  
              run: echo " my fist github action job"  

            - name : list files
              run: ls

            - name: read file
              run: cat README.md 

</pre>

 ## About action checkout uses : actions/checkout@v4
  What it does, it checkout your repository code into the github action runner,  
  it ensures the runner has exact commit that triggered workflow.  

  It clones the repo to runner  






