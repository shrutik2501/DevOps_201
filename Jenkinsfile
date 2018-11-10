pipeline {
	agent any
	stages{
			stage('Build'){
				steps{
					sh 'mvn clean package'
				}
				post{
					success{
						echo 'Now storing binary..'
						archiveArtifacts artifacts: '**/target/*.war'
					}
				}
			}
		}
	}