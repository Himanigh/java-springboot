pipeline {
agent any
stages {
    
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
    
    stage('Deploy to Dev')
    {
        steps
        {
            echo 'Deploy to Dev'
        }
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