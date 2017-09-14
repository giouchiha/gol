// start of pipeline 
pipeline {  
  // where pipeline job will run  
  agent any  
  // start of stages : build, test, deploy ...  
  stages {    
    // start of stage : build    
    stage('build') {      
      // start of running steps inside one stage      
      steps {        
        // invoke command to build with maven
        bat 'mvn clean install'      
      }    
    }  
  } 
}

// This shows a simple build wrapper example, using the AnsiColor plugin.
node {
    // This displays colors using the 'xterm' ansi color map.
    ansiColor('xterm') {
        // Just some echoes to show the ANSI color.
        stage "\u001B[31mI'm Red\u001B[0m Now not"
    }
}
