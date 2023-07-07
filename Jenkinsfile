pipeline{
	agent any
	stages{
		stage('1-clonecode'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-creds', url: 'https://github.com/enwokocha/team6-demo1.git']])
			}
		}
		stage('2-s2'){
			steps{
				sh 'lscpu'
				sh 'whoami'
			}
		}
		stage('3-s3'){
			steps{
				sh 'df -h'
				sh 'touch team6'
			}
		}
		stage('4-s4'){
			steps{
				sh 'pwd'
				sh 'du -h'				
			}
		}
        stage('5-s5'){
            steps{
                echo "Welcome to Jenkinsfile"
            }
        }
        stage('6-scripting'){
            steps{
                sh 'bash -x /var/lib/jenkins/workspace/team6-demo1-pipeline/scripting.sh'
            }
        }
	}
}