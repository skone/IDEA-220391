# IDEA-220391
Sample project to demonstrate the issue https://youtrack.jetbrains.com/issue/IDEA-220391

git clone git@github.com:skone/IDEA-220391.git
 open intellij
 file -> new project -> new empty project
 set the location of the empty project to be the cloned project directory
 Cancel the project structure window and then import the modules.

 file -> new module from existing sources -> navigate to the projectA folder
 select import module from external module -> gradle

  file -> new module from existing sources -> navigate to the projectB folder
 select import module from external module -> gradle



Open libraryTest.java in projectA it compiles OK in Intellij
Then open LibraryTest in projectB the junit dependencies aren't being found

N.B. Project B  includes Project A in the settings.gradle file
