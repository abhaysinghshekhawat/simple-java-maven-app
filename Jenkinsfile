pipeline{
  agent any
  stages{
    stage('testing'){
      steps{
        echo "hello"
        sh "pwd"
        sh "ls"
        sh "sudo cat pom.xml"
        git 'https://github.com/abhaysinghshekhawat/loadbalancer_setup.git'
        stash includes: '*' , name: 'myapp'
        sh "ls"
      }
    }
      stage('testing2'){
        steps{ 
          untash 'myapp'
          sh "ls"
          git 'https://github.com/abhaysinghshekhawat/hdfs_mapred_cluster.git'
          sh "ls"
          sh "pwd"
        }
      }
          
    }
  }

