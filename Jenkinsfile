#! /usr/bin/groovy
import jenkins.model.*

jenkins = Jenkins.instance

@Library('my-shared-lib')_
node {
   load "/src/build-version.properties"
   sh 'cat build-version.properties'
}
