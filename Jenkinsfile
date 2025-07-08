pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        git url: 'https://github.com/JAVELIN123/public.git', branch: 'main'
      }
    }

    // Xóa hoặc comment stage này:
    // stage('Install & Test') {
    //   steps {
    //     sh 'npm install'
    //   }
    // }

    // Nếu muốn test nhanh, thay bằng:
    stage('Skip Tests') {
      steps {
        echo 'No package.json present, skipping npm install'
      }
    }
  }
}
