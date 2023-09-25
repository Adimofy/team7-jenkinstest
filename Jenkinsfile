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
				sh 'dh -h'
			}
		}
		stage('3-unitest'){
			steps{
				sh 'lscpu'
			}
		}
	}	
}