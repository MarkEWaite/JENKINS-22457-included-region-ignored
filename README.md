Included region ignored
=======================

[JENKINS-22457](https://issues.jenkins-ci.org/browse/JENKINS-22457)
reports that included regions were not matched yet a build was still
triggered.  This repository attempts to duplicate the case.

I was unable to duplicate the problem.  I made changes in the build
directory and in the root directory.  They were correctly ignored.  I
made a change in the scripts directory.  It was correctly detected.

I switched the job definition from using a git URL to use an ssh URL.
Still the same behavior.
