
node 
{   
   stage('scm checkout') { 
      
      git 'https://github.com/devopsmastek/Auto.git'
     
     
   }
  
  
   stage ('deploy')
          {
    sh  "pwd"    
    def TARGET_IP = params.TARGET
    print "DEBUG: parameter foo = ${TARGET}"
             
             if ( ${DEPLOY_TO_DEV} == 'true') {
    def source = "/var/lib/jenkins/workspace/autoscaling_project/*.html}"
    def  destination = "/var/lib/tomcat8/webapps/"
         sshagent(['ubuntu']) {
        sh "scp -o StrictHostKeyChecking=no /var/lib/jenkins/workspace/autoscaling_project/*.html ubuntu@${TARGET}:/var/www/html/"
}                    
             }                           
        }
      
   }
