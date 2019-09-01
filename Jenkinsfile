
node 
{   
   stage('scm checkout') { 
      
      git 'https://github.com/devopsmastek/Auto.git'
     
     
   }
  
  
   stage ('deploy')
          {
    sh  "pwd"    
    def source = "/var/lib/jenkins/workspace/java_app_cloud_sonar/target/*.war}"
    def  destination = "/var/lib/tomcat8/webapps/"
    sh "cp -r /var/lib/jenkins/workspace/java_app_cloud_sonar/target/*.war ${destination} "
      
        }
      
   }
