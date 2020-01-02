# jenkins

Jenkins have two types of pipelines :
1. declarative pipeline
2. scripted pipeline

# How to use tools in scripted  pipelines

 test = tool name: 'node', type: 'nodejs'  
 test1 = tool name: 'mvn', type: 'maven'
 
 test is a variable
 tool name is a name that is defained in manager jenkins, global tool configuration type is nodejs
 
 now it's time to call this plugin in shell
 
 sh "${test}/bin/node -v"
 sh "${test1}/bin/mvn -v"
 
 for reference you can check Jenkinsfiles
 
 # How to use tools in declarative pipeline
 
 tools {
      nodejs "toolname" //tool name from global tool configuration
      maven "mvn"
      }
 
 call plugin
 
 sh 'mvn -v'
