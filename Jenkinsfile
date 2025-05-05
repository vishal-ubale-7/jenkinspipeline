pipeline
{
    agent any
   parameters 
   {
    string(name: 'Person', defaultValue: 'vishal ubale', description: 'How Are you')
    booleanParam(name: 'Male', defaultValue: 'true', description: '')
    choice(name: 'City', choices: ['Pune', 'Mumbai', 'Jaipur'], description: 'Select Your City')
    choice(name: 'Devoleper', choices: ['Python', 'Java', 'React'], description: 'Select Your Language')
    choice(name: 'Employee', choices: ['Microsoft', 'Google', 'EY'], description: 'Select Your Company')
    choice(name: 'Experience', choices: ['1Y', '2Y', '3Y','>3'], description: 'How Many Experience')

}
    stages 
    {
        stage('Test') 
        {
            steps 
            {
             echo 'test'
            echo "Hello from Groovy: ${params.Person}"
             bat 'echo Windows batch output: %person%'

            }
        }
                stage('Build')
                {
            steps
            {
                echo 'build'
            }
        }
                stage('Deploy on test')
                {
            steps
            {
                echo 'deploy on test'
            }
        }
                stage('Deploly on prod')
                {
            steps
            {
                echo 'deploy on prod'
            }
        }
    }
    post{
    always { 
            echo 'I will always say Hello again!'   
          }
  }
}
 
