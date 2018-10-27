#! /usr/bin/groovy
import jenkins.model.*
jenkins = Jenkins.instance

@Library('my-shared-lib')_
node {
   git branch: master, url: 'https://github.com/sarathp12/test_logic.git' 
   load 'build-version-properties'
   getMmbpValues
}
