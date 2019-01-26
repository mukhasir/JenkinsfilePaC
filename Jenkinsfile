pipeline{
	agent {
		label 'master'
	}
	stages{
		stage('SCM'){
			steps{
				echo 'Checking Out'
				checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'Mukhasir_Github', url: 'git@github.com:mukhasir/JenkinsfilePaC.git']]])
			}
		}
		stage('Second'){
			steps{
				echo 'Second'
			}
		}
	}
}