node('master'){
stage('first test')
{
    test = tool name: 'mvn'
    test1 = tool name: 'node', type: 'nodejs'
    sh "${test}/bin/mvn -v"
    sh "${test1}/bin/node -v"
    }
}
