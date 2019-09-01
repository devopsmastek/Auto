
node 
{   
   stage('scm checkout') { 
      
      git 'https://github.com/devopsmastek/Auto.git'
     
     
   }
  
  
   stage ('deploy')
          {
    sh  "pwd"    
    def TARGET_IP = env.$TARGET_IP
    print "DEBUG: parameter foo = env.TARGET_IP"
    def source = "/var/lib/jenkins/workspace/autoscaling_project/*.html}"
    def  destination = "/var/lib/tomcat8/webapps/"
    sh "cp -r /var/lib/jenkins/workspace/autoscaling_project/*.html $(TARGET_IP)/var/lib/jenkins "
      
        }
      
   }
