pipeline{
  agent any
  stages{
    stage('testing'){
      steps{
        echo "hello"
        sh "pwd"
        sh "sudo cat pom.xml"
      }
    }
      stage('testing2'){
        steps{ 
          git 'https://github.com/abhaysinghshekhawat/hdfs_mapred_cluster.git'
          sh "ls"
          sh "pwd"
        }
      }
          
    }
  }

