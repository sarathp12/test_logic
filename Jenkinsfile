#! /usr/bin/groovy

node {

   def file = "/var/lib/jenkins/workspace/test_logic/build-version.properties"
   def getMmpbValues = {
               Properties proplist = new Properties()
               File proplistFile = new File("$file")
               proplistFile.withInputStream {
               proplist.load(it)
                 }
               y = proplist
    }
   getMmpbValues()
   println y
}
