**JGit binary repository**

Updating
--------

To update the files, you need to follow the steps below:

* Grab latest JSch release and run the tests in Eclipse.`
* Modify Session.java : 141, set daemon_thread=true.
* Export JSch to a .jar file.

* Grab latest JGit master and run the tests in Eclipse.`
* Apply jgit.patch.
* Export org.eclipse.jgit to a .jar file.
* Export org.eclipse.jgit.test and org.eclipse.jgit.junit to a .jar file.

* Grab the latest JUnit and Hamcrest core Jars.
* Run `ikvmc.exe -sharedclassloader -target:library jgit.jar jsch.jar jgit-test.jar junit.jar hamcrest-core.jar`.
* Replace binaries in the repository and run MonoDevelop tests.
