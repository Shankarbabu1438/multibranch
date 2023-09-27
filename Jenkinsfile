node('buit-in') 
{
    stage('Continuous Download_child') 
	{
    git 'https://github.com/KranthiGajjelli/Maven.git'
	}
    stage('Continuous Build_child') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment_child') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war   ubuntu@172.31.26.217:/var/lib/tomcat8/webapps/qaenv.war'
	}

}
