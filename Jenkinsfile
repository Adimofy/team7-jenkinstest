pipeline{
	agent any
	stages{
		stage('1-clonecode'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'team7-git-id', url: 'https://github.com/Adimofy/team7-jenkinstest.git']])
			}
		}
		stage('2-artifactbuild'){
			steps{
				sh 'df -h'
			}
		}
		stage('3-unitest'){
			steps{
				sh 'lscpu'
			}
		}
        stage('3-unitest'){
			steps{
				echo "we are on pipeline as code module"
			}
		}
	}	
}