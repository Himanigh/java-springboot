pipeline {
agent any
stages {
    #CI
    stage('Build')
    {
        steps
        {
            echo 'Build'
        }
    }
    stage('Test')
    {
        steps
        {
            echo 'test'
        }

    }
     stage('Quality Gate-Sonar Cube')
     {
        steps
        { 
            echo 'Quality Sonar Cube'
        }

     }
     #CD
    stage('Deploy to Dev')
    {
        steps
        {
            echo 'Deploy to Dev'
        }
    }
    stage('Deploy to QA')
    {
        steps
        {
            echo 'Deploy to QA'
        }
    }
    stage('Deploy to UAT')
    {
        steps
        {
            echo 'UAT'
        }
    }
    stage('Deploy to Prod')
    {
        steps
        {
             echo 'Prod'
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