#! /usr/bin/groovy
import jenkins.model.*
import java.io.File;
import java.util.*;
jenkins = Jenkins.instance

@Library('my-shared-lib')_

properties = null

node {
   checkout scm
   load 'build-version.properties'   
   Properties proplist = new Properties()
   File proplistFile = new File("${workspace}/build-version.properties")
   proplistFile.withInputStream {
          proplist.load(it)
          }
   x = proplist
   println x
   sh 'cat build-version.properties'
}
