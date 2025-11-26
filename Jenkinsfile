pipeline{
    agent any

    environment {
        VERCEL_TOKEN = credentials('vercel-token')
    }
    stages{
        stage("Install"){
            steps{
                bat 'npm install'
            }
        }

        stage("Test"){
            steps{
               echo 'No Test yet'
            }
        }
        stage("Build"){
            steps{
                bat 'npm run build'
            }
        }
        stage("Deploy to vercel"){
            steps{
                bat 'npx vercel --prod --token=9yOUKVzSIAu2tyXZ4ArwPjK3 --yes'
            }
        }
    }
}