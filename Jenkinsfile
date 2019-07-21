pipeline { 
agent any
stages {
stage ('SCM'){
steps { git 'https://github.com/Bhagya1707/warfileFinal.git'     }
}
stage ('build'){
steps {  bat label: '', script: 'mvn clean'
bat label: '', script: 'mvn install'   }
}
stage ('dep[loy'){
steps { bat label: '', script: 'xcopy /y "C:\\Program Files (x86)\\Jenkins\\workspace\\pipeline2\\target\\demobranch.war"  "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'
       }
}
}
}
