
node 
{   
   stage('scm checkout') { 
      
      git 'https://github.com/devopsmastek/Auto.git'
     
     
   }
  
  
   stage ('deploy')
          {
    sh  "pwd"    
    def TARGET_IP = params.TARGET
    sh " echo '$TARGET_IP'"
    print "DEBUG: parameter foo = ${TARGET}"
    def source = "/var/lib/jenkins/workspace/autoscaling_project/*.html}"
    def  destination = "/var/lib/tomcat8/webapps/"
    sh "cp -r /var/lib/jenkins/workspace/autoscaling_project/*.html /var/lib/jenkins "
      
        }
      
   }
