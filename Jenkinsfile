#! /usr/bin/groovy
import jenkins.model.*
jenkins = Jenkins.instance

node {
   git branch: master, url: 'https://github.com/sarathp12/test_logic.git' 
   load 'build-version-properties'

   def getMmpbValues = {
             Properties proplist = new Properties()
             File proplistFile = new File('build-version.properties')
             proplistFile.withInputStream {
                 proplist.load(it)
                }
             x = proplist
    }  
   stage('print') {
       println x
   }
}
