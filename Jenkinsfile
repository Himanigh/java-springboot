pipeline {
agent any
stages {
    
    stage('Build')
    {
        steps
        {
            echo 'Build'
            sh 'mvn clean package'
        }
    }
    stage('Test')
    {
        steps
        {
            echo 'test'
            sh 'mvn test'
        }

    }
     stage('Quality Gate-Sonar Cube')
     {
        steps
        { 
            echo 'Quality Sonar Cube'
        }

     }
    
    stage('Deploy to Dev')
    {
        steps
        {
            echo 'Deploy to Dev now'
        }
    }

    }
   


post{
    failure{
        echo 'failed'
    }
    success{
        echo 'success'
    }
    always{
        echo 'always'
    }

}
}