pipeline 
{
    agent any

    stages 
    {
        stage('Checkout SCM') 
        {
            steps 
            {
                git branch: 'main', credentialsId: 'Checkout', url: 'https://github.com/aqsa286/Checkout_scm_jenkinsfile.git'
            }
        }   
    }
    post
    {
        always
        {
            emailext body: 'Summary', subject: 'Checkout Scm', to: 'aqsafarooq402@gmail.com'
        }
    }
}
