pipeline {
	agent any

	node {
		

	stages {
		stage('checkuou') (
                    scm 	https://github.com/NiceGuyFirst/Oren1.git
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
