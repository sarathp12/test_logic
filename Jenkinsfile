#! /usr/bin/groovy

@Library('my-shared-lib')_


node {
   load 'build-version.properties'   
   sh 'cat build-version.properties'

   //file read step
   properties = new Properties()
   File propertiesFile = new File("${workspace}/build-version.properties")
   propertiesFile.withInputStream {
      properties.load(it)
    }
   //con.close();
   x = proplist
   println x
 //con.close();
 }
