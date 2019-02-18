def workspace;
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sowmithracha/myproj.git']]])
        workspace = pwd()
    }
    stage('Statis code analysis')
    {
        echo "Static code analysis"
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage('code test')
    {
        echo "unit testing"
    }
    stage('delivery')
    {
        echo "delivery th code"
    }
}
