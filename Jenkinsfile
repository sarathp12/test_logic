#! /usr/bin/groovy

@Library('my-shared-lib')_


node {
   //file read step
   Properties properties = new Properties()
   File propertiesFile = new File("${workspace}/build-version.properties")
   propertiesFile.withInputStream {
      properties.load(it)
    }
   //con.close();
   x = properties
   println x
 //con.close();
}
