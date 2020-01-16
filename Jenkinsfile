properties([[$class: 'JiraProjectProperty'], pipelineTriggers([pollSCM('30 * * * *')])])
node {
    stage("checkout"){
        git "https://github.com/MorLiberty/MySoftware.git"
    }
    stage("test"){
        bat label: '', script: 'master.py'
    }
}