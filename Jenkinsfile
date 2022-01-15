node{
    
    stage('Cloning'){
        git branch: 'main', credentialsId: 'raghuveerat713', url: 'https://github.com/RaghuveerT1994/demo.git'
        //git branch: 'main', credentialsId: 'raghuveerat713', url: 'https://github.com/RaghuveerT1994/demo.git
    }
    
    stage('check'){
        sh 'ls'
    }
    
    stage('pushing to remote server'){
        //sh 'sshpass -p "123qwer" scp creating_file.sh ubuntu@172.31.14.27:~/raghu/.'
        sh 'sshpass -p "123qwer" scp creating_file.sh ubuntu@172.31.14.27:~/raghu/.'
    }
    
    stage('executing shell file'){
        sh 'sshpass -p "123qwer" ssh ubuntu@172.31.14.27  /bin/bash ./raghu/creating_file.sh'
    }
    
}
