# Introduction #

This page describes how to download the Martus source code, It is for developers who want to contribute code to the Martus project.

**NOTE: These instructions have not yet been tested, so might be inaccurate**

# System Requirements #

  * Java 1.5+
  * Eclipse Indigo
  * EclipseMercurial plugin
  * Server: Linux
  * Client: Windows, Mac, or Linux

# Downloading #

1. In Eclipse, create a new workspace.

2. In the Package Explorer view, do a right-click/Import/Mercurial/Clone Existing Mercurial Repository.

3. For the URL, enter:
  * https://code.google.com/p/martus.martus-amplifier/

4. Hit OK

5. Repeat steps 2-4 for each of the following URLs:
  * https://code.google.com/p/martus.martus-amplifier/
  * https://code.google.com/p/martus.martus-bc-jce/
  * https://code.google.com/p/martus.martus-client/
  * https://code.google.com/p/martus.martus-clientside/
  * https://code.google.com/p/martus.martus-common/
  * https://code.google.com/p/martus.martus-docs/
  * https://code.google.com/p/martus.martus-hrdag/
  * https://code.google.com/p/martus.martus-jar-verifier/
  * https://code.google.com/p/martus.martus-csv2xml/
  * https://code.google.com/p/martus.martus-logi/
  * https://code.google.com/p/martus.martus-meta/
  * https://code.google.com/p/martus.martus-mspa/
  * https://code.google.com/p/martus.martus-server/
  * https://code.google.com/p/martus.martus-swing/
  * https://code.google.com/p/martus.martus-thirdparty/
  * https://code.google.com/p/martus.martus-utils/

6. Right-click on martus-csv2xml, and to a Refactor/Rename, and change the name to martus-js-xml-generator

# Configuring the projects in eclipse #

1. Go to Window/Preferences/Java/Installed JRE's.
  * Select the JRE and choose Edit
  * Choose Add External Jars..
  * Select the bc-jce.jar file from inside the bc-jce project you checked out earlier.
  * Select bc-jce.jar in the list, and use the Up button to move it above jsse.jar

At this point, the project should compile without errors.

# Running tests #

1. Hit Ctrl-Shift-T and enter "TestAllQuick".

2. When it comes up, hit Run/Run As... Junit Test. All tests should pass.