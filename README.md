# kotlin-notes
------------------------------------------

Kotlin setup in eclipse:
------------------------------
     1) install kotlin plugin using marketplace search by kotlin keyword.
     2) create maven project select kotlin archetype called--kotlin-archetype-jvm (for standalone)
      if this archetype is not present in catalog please add this archetype using following values
           Archetype Group Id =org.jetbrains.kotlin
           Archetype Artifact Id =kotlin-archetype-jvm
           Archetype Version =1.3.41
           Repository URL = https://repo1.maven.org/maven2
      or you can search in maven for latest version
 
 
 
 Basic of Kotlin
 -----------------
 
 code structure
 ---------------
      package .....
      import....

      class {
      ;;;;;
      }
      member ----
      method ....
 
 wrting class is not mandatory to write any method or variable.you can directly write method
 this type of method and variable is called top level member which is accessible for all class of same package.
 
 in kotlin you can import method and variable also along with class
 
 
 Variable:
 -----------
      Syntax to write variable
      var/val name :[data-type] = value;
      val is use for final value
      and var is use for variable
      Example:
      var age = 25;
      var name = "Amir";
      val index = 100;

 
 Function in kotlin
 --------------------
       using fun keywords

       fun function_name (parameters): [return_type]{
       //body
       }

      example of main function
      ---------------------------

      fun main(args:Array<String>)
       {
       println("hello world");   
      }

      default value of return_type is unit

      fun findAge(): Int {
      return 10;
      }

 
 
 
 Scripting in Kotlin
 -----------------------
      its just like main method body along with import statement. file extension will be kts
      to run script file you first need to setup kotlin setup 
      1) download kotlin-compiler-1.3.41.zip
      https://github.com/JetBrains/kotlin/releases/tag/v1.3.41 
      2) set path varialbe to bin dir
 
 how to write kotlin script (test.kts)
 ----------------------------------
 
      import java.io.File
     var name = "String"
          var myname : String  = "Amir"
         println(name);
           println(myname);
          println("Hello, World");

          if (myname.equals("Amir")) {
               println("names are same");
          }

     val folders = File(args[0]).listFiles { file -> file.isDirectory() }
     folders?.forEach { folder -> println(folder) }
      save test.kts 

      run using following command
      kotlinc -script test.kts C:\Users\inkajm01

      C:\Users\inkajm01 is command line argument

      basic syntax is  kotlinc -script test.kts


      to compile kts or kt file
          kotlinc  test.kts

 
 
 
 
 
 
 
 
 
 
 
 
 
