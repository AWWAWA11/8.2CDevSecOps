pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo "Stage 1: Build using tool = Maven"
      }
    }

    stage('Unit and Integration Tests') {
      steps {
        echo "Stage 2: Unit tests tool = JUnit"
        echo "Stage 2: Integration tests tool = Testcontainers"
      }
    }

    stage('Code Analysis') {
      steps {
        echo "Stage 3: Code analysis tool = SonarQube (SonarQube Scanner)"
      }
    }

    stage('Security Scan') {
      steps {
        echo "Stage 4: Security scan tool = OWASP Dependency-Check"
      }
    }

    stage('Deploy to Staging') {
      steps {
        echo "Stage 5: Deploy to staging (AWS EC2) tool = AWS CLI"
      }
    }

    stage('Integration Tests on Staging') {
      steps {
        echo "Stage 6: Staging integration tests tool = Postman/Newman"
      }
    }

    stage('Deploy to Production') {
      steps {
        echo "Stage 7: Deploy to production (AWS EC2) tool = AWS CLI"
      }
    }
  }
}
