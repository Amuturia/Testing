pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                mail bcc: '', 
		body: 'If you are reading this then you must have done the Blueocean pipeline creation correctly.', 
		subject: 'BlueOcean Test', 
		to: 'antony.muturia@student.moringaschool.com'
            }
        }
    }
}