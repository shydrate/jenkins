node('master'){
stage('first test')
{
    test = tool name: 'mvn'  //tool name will be pickup from global tool configuration
    test1 = tool name: 'node', type: 'nodejs'   //tool name will be pickup from global tool configuration
    sh "${test}/bin/mvn -v"
    sh "${test1}/bin/node -v"
    }
}
