# RESTful Web Services

### Date:

## Aim

To create RESTful web services using both server-side and client-side implementations.

## Procedure

### Server-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Web Services:**
   - Right-click on the project name and select `New` -> `RESTful Web Services from Patterns`.
     ![image](https://github.com/user-attachments/assets/4c246ecc-e1d7-45d1-970a-854dcdc28736)


3. **Configure Resource:**
   - In the new window, select `Simple Root Resource` and click `Next`.
   - Provide a Resource Package name and choose `MIME Type` as `text/html`. Click `Finish`.
     ![image](https://github.com/user-attachments/assets/55fd4817-d869-4b4e-94ac-457c4a9bd390)


4. **Edit Resource:**
   - Two editing tabs will appear. Close `ApplicationConfig.java` and implement the required functionalities in `GenericResource.java`.
     ![image](https://github.com/user-attachments/assets/cef254e9-45db-4660-b1ea-01d3328e7ee1)


5. **Modify Method:**
   - Alter the `getHtml()` method as needed.

6. **Build and Deploy:**
   - Save your project, clean and build it. Deploy your project to the server.
   - ![image](https://github.com/user-attachments/assets/8722da37-9b0d-49b1-b5f5-d72f092a203b)


7. **Test Your Web Service:**
   - Open a browser and type the URL `http://localhost:8080/project_name/webresources/generic?params=45&params=35` to test the web service functionality.

### Client-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Java Client:**
   - Right-click on the project and select `New` -> `RESTful Java Client`.
     ![image](https://github.com/user-attachments/assets/4d0066f0-975c-45e2-b66b-6b9f422905e2)


3. **Configure Client:**
   - In the new window, provide a name for your client, a package name, and select `From Project` under the `Select the REST resource:` tab. Click `Browse` and select your RESTful resource. Click `OK`, then `Finish`.

4. **Edit Client Code:**
   - Modify the `getHtml()` method as required.
     ![image](https://github.com/user-attachments/assets/5d537bd1-4b0c-40cc-b6bb-20b9058c8ba2)


5. **Add JAR File:**
   - Right-click on the `Libraries` folder under your project and select `Add JAR/Folder`.
   - Navigate to where the `javax.ws.rs-api2.0.1.jar` file is located and add it.
     ![image](https://github.com/user-attachments/assets/09f658dc-8046-4df6-9f29-b5d8c5bff358)


6. **Create JSP Page:**
   - Right-click on the `Web Pages` folder and select `JSP`.
   - Provide a name for the JSP page and click `Finish`.
     ![image](https://github.com/user-attachments/assets/bd3e1ef3-00fb-457c-ae8a-54a8034eb1d1)


7. **Include Client Code in JSP:**
   - Edit the JSP page to include the necessary code for invoking the client Java code.
     ![image](https://github.com/user-attachments/assets/f7b5695f-c4f3-47b6-82fb-5df7a8b4ab52)


8. **Build and Run:**
   - Save the project, build it, and run the JSP file to see the output in a new browser window.
     ![image](https://github.com/user-attachments/assets/9506ba81-47b7-49e3-88b6-b3d5a46f9eff)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a 
name to the JSP page and click Finish. 

Step 10: A new tab will appear with the default contents of the JSP page. In that, include 
at the top and type the following code to invoke the client java code. 

![image](https://github.com/user-attachments/assets/5a734882-7282-4eea-b702-04ebf36b476c)

Step 11: Save the project and build it. 
Step 12: Run the JSP file and you should see the output in a new browser window.

![image](https://github.com/user-attachments/assets/6669e150-ebd7-4826-bca8-8f8decff85a1)



### Client-Side Remote Invocation (Optional)

1. **Adjust Client Configuration:**
   - Follow steps 1-5 from the Client-Side Implementation.
   - In the generated `NewJerseyClient.java` file, update `BASE_URI` from `private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources";` to `private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";`.

2. **Complete the Remaining Steps:**
   - Follow steps 6-12 from the Client-Side Implementation to finalize and test the remote client.

## Result

The implementation of RESTful web services using both server-side and client-side components was successfully created and executed.

