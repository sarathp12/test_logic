#! /usr/bin/groovy
import jenkins.model.*
import java.io.File;
import java.util.*;


@Library('my-shared-lib')_


node {
   load 'build-version.properties'   
   sh 'cat build-version.properties'

   //file read step
   Properties proplist = new Properties()
   File proplistFile = new File('build-version.properties')
   proplistFile.withInputStream {
      proplist.load(it)
   }
   x = proplist
   println x
}
