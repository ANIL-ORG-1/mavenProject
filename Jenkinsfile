node('master')
{
    stage('ContinuousDownload_Master') 
    {
        git 'https://github.com/intelliqittrainings/maven.git'
    }
    stage('ContinuousBuild_Master')
    {
        sh label: '', script: 'mvn package'
    }
    }
