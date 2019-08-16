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
  
  fun function_name (parameters) {
  //body
  }
 
 example of main function
 
 fun main(args:Array<String>)
  {
  println("hello world");   
 }
 
 
 
 
 
 
 
 
 
