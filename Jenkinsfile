properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){
      pip install ansible
      ansible-playbook -C deploy.yml
      } 
     
}
