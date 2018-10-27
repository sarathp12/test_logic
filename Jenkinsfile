#! /usr/bin/groovy

node {
   def getMmpbValues = {
               Properties proplist = new Properties()
               File proplistFile = new File('build-version.properties')
               proplistFile.withInputStream {
               proplist.load(it)
                 }
               return proplist
    }
   
   def y = proplist
   println y
}
