pipeline {
	agent any
	stages {
		stage(build) {
			steps {
				sh ./start_build.sh
			}
		}
		stage(test) {
			steps {
				python unittest.py
			}
		}
		stage(deploy) {
			steps {
				sh ./deploy.sh
				}
			}	
	}
}
