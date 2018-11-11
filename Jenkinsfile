pipeline {
	agent any
	stages{
	
		stage('Initialation'){
				steps{
					echo "I am shruti and testing jenkins.."
				}
			}
			stage('Build'){
				steps{
					bat 'mvn clean package'
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