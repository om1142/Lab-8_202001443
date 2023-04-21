# Name: Om Limbachiya
# ID: 202001443
# Subject: IT314 Software Engineering

<br>

# Lab 8: Unit Testing with jUnit
<br><br>

**1. Create a new Eclipse project, and within the project create a package.**
<br>      Created a project in Ecliplse and named the package as **JUnit**.
<br><br><br>
**2. Create a class for a Boa.**
<br>      
<br>
![image](https://user-images.githubusercontent.com/83654071/233593309-f3455db9-1d82-4fb8-b3fa-0c88f6b2024d.png)

<br><br>


**Lab Exercise:**  

**1. Create a new Eclipse project, and within the project create a package.**  
![image](https://user-images.githubusercontent.com/83654071/233594909-29f6d315-ad59-484f-bf3c-64f0080bb045.png)
![image](https://user-images.githubusercontent.com/83654071/233594952-889d5083-c0c7-4fcd-b536-6fed4802093d.png)

**2. Create a class for a Boa.**  
![image](https://user-images.githubusercontent.com/83654071/233595029-a72e02ad-6965-40bc-994d-693f82de2c2b.png)

**3. Follow the instructions in the JUnit tutorial in the section “Creating a JUnit Test Case in Eclipse”. You’ll be creating a test case for the class Boa. When you’re asked to select test method stubs, select both isHealthy() and fitsInCage(int).**

**Test Case Code:**  
![image](https://user-images.githubusercontent.com/83654071/233595190-58968d0b-fd65-4a69-958b-bbd250fc21be.png)

**4. Now it’s time to write some unit tests. Notice that the BoaTest class that JUnit created for you contains stubs for several methods. The first stub (for the method setUp()) is annotated with @Before. The @Before annotation denotes that the method setUp() will be run prior to the execution of each test method. setUp() is typically used to initialize data needed by each test. Modify the setUp() method so that it creates a couple of Boa objects, as follows:**  
![image](https://user-images.githubusercontent.com/83654071/233595312-b1cb00d9-3a31-4292-b781-ad270889de86.png)

**Test Case Code:**  
![image](https://user-images.githubusercontent.com/83654071/233595375-dc871acc-db69-40e1-8668-51398fcead2f.png)

**5. JUnit also provided stubs for two test methods, each annotated with @Test. Work on the testIsHealthy() method first. The purpose of this method is to check that the isHealthy() method in the Boa class behaves the way it’s supposed to. In the JUnit tutorial, read the section on “Writing Tests”. Modify the testIsHealthy() method so that it checks the results of activating the isHealthy() method on the two Boa objects you created in setup(). Likewise, modify the testFitsInCage() method to test the results of that method. Make sure your test is robust; it should check the results when the cage length is less than the length of the boa, when the cage length is equal to the length of the boa, and when the cage length is greater than the length of the boa. Should you write tests for both jen and ken?**  
**Ans:** Yes, We should write tests for both Ken and Jen.

**6. Now you can run your tests. Read the section “Running Your Test Case” in the tutorial. Did you get a green bar in the JUnit pane? If you got a red bar, use the output in the JUnit pane to determine which test(s) failed. Fix your tests, and try running the test case again. It’s important to note that a red bar doesn’t necessarily mean that the test case is written incorrectly; it could be that the method that’s being tested isn’t correct. In fact, that’s what unit testing is supposed to do – help us find errors in our code. When a test fails, you need to determine if the error is in the test case itself or in the code it’s testing.**    

**Test Case Code**  
![image](https://user-images.githubusercontent.com/83654071/233595427-44438ffd-70bf-48f3-a9a7-e445c08a3c67.png)

**7. Add a new method to the Boa class, with this purpose and signature: // produces the length of the Boa in inches public int lengthInInches(){ // you need to write the body of this method } Add a new test case to the BoaTest class that tests the lengthInInches() method. Make sure you annotate the new test method with @Test. Run your tests.**  

**Function added in the Boa Class:**  
![image](https://user-images.githubusercontent.com/83654071/233595482-c99bbc1c-022b-44cb-80d2-3a1779f6bf94.png)

**Test Case Code:**  
![image](https://user-images.githubusercontent.com/83654071/233595516-39dc3d88-5b33-42bc-a763-a2c1f121e052.png)
