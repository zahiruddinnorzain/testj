pipeline{
	agent any

	stages {
		stage ('Compile Stage') {
			steps {
					sh 'cd /home/zebo/code/temp/',
					sh 'git clone https://github.com/zahiruddinnorzain/testj.git'
			}
		}
		stage ('Testing Stage') {
			steps {
					sh 'cd /home/zebo/code/temp/testj/'
					sh 'python3 main.py'
			}
		}
		stage ('Deployment Stage') {
			steps {
					sh 'touch 2.txt'
			}
		}
	}
}