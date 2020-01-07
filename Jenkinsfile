node('master')
{
    stage('ContinuousDownload_Loans') 
    {
        git 'https://github.com/intelliqittrainings/maven.git'
    }
    stage('ContinuousBuild_Loans')
    {
        sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_Loans')
    {
        sh label: '', script: '''scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.92.93:/var/lib/tomcat8/webapps/testapp.war
'''
    }
    
   } 
    
    
    
    
    
    
    
    

