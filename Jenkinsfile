#! /usr/bin/groovy
import jenkins.model.*
jenkins = Jenkins.instance

node {
   git branch: master, url: 'https://github.com/sarathp12/test_logic.git' 
   load 'build-version-properties'

   /*
   def getmmpbValues = {
       proplist = new Properties()
       File proplistFile = new File("build-version-properties")
       proplistFile.withInputStream {
          proplist.load(it)
          }
       return proplist
    }
    
   def y = getMmpbValues()
   println y
   */
  stages {
    stage ('Mmbp Values') {
       steps {
           def getMmpbValues = {
             Properties proplist = new Properties()
             File proplistFile = new File('build-version.properties')
             proplistFile.withInputStream {
                 proplist.load(it)
                }
             x = proplist
           }  
       }       
    }  
    stage ('print outs') {
       steps {
          println getMmpbValues()
          println x
          println x.minor
       } 
    }
    stage ('iteration') {
        steps {
           x.each { key, value ->
           println "$value.$value.$value.$value"
           } 
        } 
    } 
    stage ('print ieration') {
       steps {
           def f = "${x.major}.${x.minor}.${x.patch}.${x.build}"
           println f
       }
    }   
 }
}

