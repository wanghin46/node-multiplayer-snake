agent any {  
    stage('Cloning Git') {
        /* Let's make sure we have the repository cloned to our workspace */
       checkout scm
    }  
    stage('SAST'){
      sh 'echo SAST stage'
    }

    
    stage('Build-and-Tag') {
    /* This builds the actual image; synonymous to
         * docker build on the command line */
      sh 'echo Build and Tag'
    }

    stage('Post-to-dockerhub') {
     sh 'echo post to dockerhub repo'
    }

    stage('SECURITY-IMAGE-SCANNER'){
     sh 'echo scan image for security'
    }

    stage('Pull-image-server') {
         sh 'echo pulling image ...'
      }
    
    stage('DAST')
        {
         sh 'echo dast scan for security'
        }
 
}
