#! /usr/bin/groovy
#
node {
   git branch: master, 'url: https://github.com/sarathp12/test_logic.git' 
   load 'build-version-properties'

   Properties proplist = new Properties()
   File proplistFile = new File("build-version-properties")
   proplistFile.withInputStream {
        proplist.load(it)
           }
   return proplist
    
   def y = getMmpbValues()
   println y
}
