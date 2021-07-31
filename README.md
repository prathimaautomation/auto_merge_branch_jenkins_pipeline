# Auto merge branch jenkins pipeline to test the app, merge the dev with main and deploy into ec2 instance

## Sparta Node Sample App


# Jenkins  Lab

## Timings
 
This lab last 30 - 60 Minutes

## Summary

* Our current CI setup on Jenkins has one major flaw. The build is currently started and the tests are run on the master branch of the repository. This means that if the tests fail the code still exists on the master branch ( which is only supposed to contain working code ).

* We need to reconfigure the job so that the code is tested on a different branch ( develop ) and automatically merged with the master branch if the tests pass.

* The developers should also be informed on Github if their commit passed the tests or not and they should be notified via email too.

## Tasks

* Configure your job to checkout code from the dev branch rather than the main branch
* Have the job merge the dev branch code with the master branch and test against that
* Use the Git publisher plugin to push the master branch to Github if the tests pass.

## Tips

* All of these items are simple configuration provided by plugins that are already installed and setup on our Jenkins instance. If you are writing code you are doing it wrong.

- You will need to research how these plugins works:

* The Github plugin
* The Git publisher plugin


