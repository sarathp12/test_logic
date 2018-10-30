#! /usr/bin/env groovy

@Library('my-shared-lib')_
import org.android.*

node {
  git url: 'https://github.com/sarathp12/test_logic.git'
  def pl = new workingMmpbValues() 
  pl.userInputRead()
  pl.valuesIncrement()
}
