# lp-java
Linear Program Solver in Java using ortools

I used the google ortools (Optimization tools) library. The library is composed of two external jar file : com.google.ortools.jar and portobuf.jar and of one native class library jniortools.dll. You can find these libraries under the folder lib. 

To see an example of how the java class should be of a simple lp, check the class SimpleLPExample under src. 
The SimpleLPExample represent the following LP: 
<p align="center">
  <img src="/img/example-lp.PNG?raw=true" alt="LP example"/>
</p>

## Command line (windows)
If you want to run the java class through command lines you should run the following commands : 
```bash
javac -d objs -cp lib/com.google.ortools.jar;lib/protobuf.jar src/SimpleLPExample.java
java -Djava.library.path=lib -cp objs;lib/com.google.ortools.jar SimpleLPExample
```

## Eclipse
If you want to run the java class in the eclipse, you should do the following steps :
You should add the 2 libraries as external libraries, by By going to the properties of the project > Libraries and click on the button Add External JARs.

After adding the 2 libraries, you should specify in the Eclipse the location of the Native Library Location. By going to the properties of the project > Java Build Path > Source Tabulation and Editing the location of Native library like the image below.
<p align="center">
  <img src="/img/Capture.PNG?raw=true" alt="step 1"/>
</p>
And then specify the location of the library folder by clicking on the External Folder button 
<p align="center">
  <img src="/img/Capture2.PNG?raw=true" alt="step 2"/>
</p>
And finally navigate through the repository and select the folder lib
<p align="center">
  <img src="/img/Capture3.PNG?raw=true" alt="step 3"/>
</p>

After including all the libraries you are to go. You can run the project inside of Eclipse.