pipeline{
  agent any  
  stages{  
      stage("Run ansible playbook"){
        steps{
        ansiblePlaybook credentialsId: 'ssh_key', inventory: 'host', playbook: 'nginx_install.yaml', vaultTmpPath: ''
        
        }
      }
  }
}
