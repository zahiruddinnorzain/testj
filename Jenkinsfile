pipeline{
	agent any

	stages {
		stage ('Compile Stage') {
			steps {
				withMaven(maven: 'maven_3_6_3'){
					sh 'python3 main.py'
				}
			}
		}
		stage ('Testing Stage') {
			steps {
				withMaven(maven: 'maven_3_6_3'){
					sh 'touch 1.txt'
				}
			}
		}
		stage ('Deployment Stage') {
			steps {
				withMaven(maven: 'maven_3_6_3'){
					sh 'touch 2.txt'
				}
			}
		}
	}
}