@Library("prasanna") _
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
              script{
                add(10,20)
                PrintNumbers()
                PrintEvenNumbers()
                def originalString = "hello world"
                def upperCaseString = toUpper(originalString)
              } 
            }
        }
    }
}
