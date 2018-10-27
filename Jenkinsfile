#! /usr/bin/groovy

node {
   def currentDir = new File(".").getAbsolutePath()
   println currentDir 
   def getMmpbValues = {
               Properties proplist = new Properties()
               File proplistFile = new File("/.build-version.properties")
               proplistFile.withInputStream {
               proplist.load(it)
                 }
               return proplist
    }
   
   def y = getMmpbValues()
   println y
}
