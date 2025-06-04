pipeline{
	agent any
	
		tools{
			maven 'maven'
			
			}
		stages{
			stage('checkout'){
				steps{
				git branch:'main' , url:'https://github.com/DivyanshuChauhan03/revisionJenkins'
				}
			}
			stage('compile and build'){
				steps{
				sh 'mvn clean install'
				}
			}
			stage('run'){
				steps{
				sh 'java -jar target/JenkinsMaven-1.0-SNAPSHOT.jar'
				}	
			}
		}
	}
