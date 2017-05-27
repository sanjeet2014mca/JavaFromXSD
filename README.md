# JavaFromXSD

Steps to generate Java classes from XSD in Eclipse :

Step 1: Create JAXB project
Open Eclipse IDE and create a new JAXB project follow File-> New -> Other -> JAXB -> JAXB Project. Select JAXB Project and click Next.

Step 2: write name of your Project

Enter the project name as JavaFromXSD and make sure jre7 is selected as the Target runtime and JAXB version as 2.2 or lower. If your project is using jre6 then you have to use JAXB version as 2.1 or base on accept and Click Next -> Next.

Step 3: JAXB Facet Setup
In JAXB Facet window, select "Generic JAXB 2.1" click Finish.

Step 4: Create XSD file

Right click on 'src' and create a new package "com.example.jaxb.schema". Now create a new XSD file inside this package. To create a new XSD file, Right click on package -> New -> Other.-> XML -> XML Schema File and click Next.

Select the location and enter the file name as 'employeers.xsd'.

 Step 5: Adding jar files to Project

We need to add  JAR files in the project classpath. which is given in project see & download according to that.
Right click on your JAXB Project-> Build Path-> Configure Build Path and select Libraries tab from right side and click on Add External JARs.Add all the jars.


Step 6: Generating Java classes
Right click on your package -> New -> Other. -> JAXB -> JAXB Classes from Schema.

Click Next and select Project (JavaFromXsd) and click Next. 
Select schema to generate classes from and click Next.

Enter the package name "com.example.jaxb.generated" for the generated Java classes and Click Next-> Next-> Finish(dont change default values while navigating).

After Finishing Click OK if you are getting any Warnings.You will see the following message displayed in the console.

You can see the generated classes in Project explorer


finally u will see........
parsing a schema... 
compiling a schema...
...........
