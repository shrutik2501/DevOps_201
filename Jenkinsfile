pipeline {
	agent any
	stages{
		stage('Initialization'){
				steps{
					echo "Initializing repsitory.."
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