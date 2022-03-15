pipeline {
  agent any
  stages {
    stage ("Deploy to K8S") {
            steps {
                script {
                   sh "export KUBECONFIG=/root/.kube/config"
                   sh "kubectl get nodes"
                   sh "kubectl apply -f /code/EKS-CODE/deployment.yaml"
                    
                }
                }
            }
		}
	}
