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
   sh 'cat build-version.properties'
}
