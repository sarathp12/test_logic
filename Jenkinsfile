#! /usr/bin/groovy

node {
   git branch: master, 'url: https://github.com/sarathp12/test_logic.git' 
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

  def getMmpbValues = {
      Properties proplist = new Properties()
      File proplistFile = new File('build-version.properties')
      proplistFile.withInputStream {
         proplist.load(it)
         }
      x = proplist
  }


  println getMmpbValues()
  println x
  println x.minor

  x.each { key, value ->
    println "$value.$value.$value.$value"
  }  

  def f = "${x.major}.${x.minor}.${x.patch}.${x.build}"
  println f
}
