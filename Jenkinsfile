#! /usr/bin/groovy

node {
   def workspace = pwd() 
   def getMmpbValues = {
               Properties proplist = new Properties()
               File proplistFile = new File("build-version-properties")
               proplistFile.withInputStream {
               proplist.load(it)
                 }
               return proplist
    }
   
   def y = getMmpbValues()
   println y
}
