pipeline {
	agent any

	node {
		

	stages {
		stage('checkuou') (
			checkout scm
		)

		stage('verify') {
			steps {
				sh 'checkmd5.sh'
				}
			}

		stage('test') {
			steps {
				sh 'python3 gethw.py > gethw.json'
				sh 'json_pp < gethw.json > /dev/null'
				}
			}
		}
           }	
				
	}
