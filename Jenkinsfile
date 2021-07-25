properties([ disableConcurrentBuilds(), pipelineTriggers([githubPush()]) ]) 
 
node{
      deleteDir()
      checkout scm

     stage('deploying stack'){
      sh 
      '''
      pip install ansible
      ansible-playbook -C deploy.yml
      '''
      } 
     
}
