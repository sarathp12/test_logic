#! /usr/bin/groovy
import jenkins.model.*

jenkins = Jenkins.instance

@Library('my-shared-lib')_
load 'build-version.properties'
node {
   sh 'cat build-version.properties'
}
