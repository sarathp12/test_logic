#! /usr/bin/groovy

node {
   def file = readFileFromWorkspace('build-version.properties')
   def getMmpbValues = {
               Properties proplist = new Properties()
               File proplistFile = new File("file")
               proplistFile.withInputStream {
               proplist.load(it)
                 }
               return proplist
    }
   
   def y = getMmpbValues()
   println y
}
