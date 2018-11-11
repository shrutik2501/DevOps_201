pipeline {
	agent any
	stages{
			stage('Init'){
				steps{
					echo "I am shruti and testing jenkins.."
				}
			}
			
			stage('Build'){
				steps{
					echo "Now Building.."
				}
			}
			
			stage('Deploy'){
				steps{
					echo "Code deployed.."
				}
			}
		}
	}
	