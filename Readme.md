# Apache Tomcat

### Step 1: Install Apache Tomcat

1. **Download Tomcat:**
   Go to the [Apache Tomcat download page](http://tomcat.apache.org/download.cgi) and download the latest stable version. Choose the Core binary distribution (ZIP or TAR.GZ).

2. **Extract the Archive:**
   Extract the downloaded archive to a directory of your choice. This will be your Tomcat installation directory.

3. **Set Environment Variables (Optional):**
   Optionally, set the `CATALINA_HOME` environment variable to point to your Tomcat installation directory. This step is not required but can be helpful.

### Step 2: Start Tomcat

1. **Navigate to the `bin` Directory:**
   Open a terminal or command prompt, navigate to the `bin` directory inside your Tomcat installation directory.

2. **Start Tomcat:**
   - On Windows: Run `startup.bat`.
   - On Unix-based systems: Run `startup.sh`.
   This will start the Tomcat server.

3. **Access Tomcat Manager (Optional):**
   Open your web browser and go to `http://localhost:8080`. If Tomcat is running, you should see the Tomcat welcome page. You can also access the Tomcat Manager at `http://localhost:8080/manager/html` (username: `admin`, password: `admin`).

### Step 3: Create a Simple Web Application

1. **Create a Web Application Directory:**
   Inside the Tomcat `webapps` directory, create a new directory for your web application. Let's name it `mywebapp`.

2. **Create a JSP File:**
   Inside the `mywebapp` directory, create a new file named `index.jsp` with the following content:

   ```jsp
   <%@ page language="java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>
   <!DOCTYPE html>
   <html>
   <head>
       <meta charset="UTF-8">
       <title>My Web Application</title>
   </head>
   <body>
       <h1>Hello, Apache Tomcat!</h1>
   </body>
   </html>
   ```

### Step 4: Deploy the Web Application

1. **Restart Tomcat:**
   If Tomcat is not already running, start it again following the instructions in Step 2.

2. **Access Your Web Application:**
   Open your web browser and go to `http://localhost:8080/mywebapp`. You should see the "Hello, Apache Tomcat!" message.

### Step 5: Stop Tomcat

1. **Navigate to the `bin` Directory:**
   Open a terminal or command prompt, navigate to the `bin` directory inside your Tomcat installation directory.

2. **Stop Tomcat:**
   - On Windows: Run `shutdown.bat`.
   - On Unix-based systems: Run `shutdown.sh`.
   This will stop the Tomcat server.


# Deploy your first JSP file

### Step 1: Create a Web Application Directory

Inside the Tomcat `webapps` directory, create a new directory for your web application. Let's name it `mywebapp`.

### Step 2: Create the JSP File

Inside the `mywebapp` directory, create a new file named `hello.jsp` with the following content:

```jsp
<%@ page language="java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Hello JSP</title>
</head>
<body>
    <h1>Hello, Apache Tomcat and JSP!</h1>
</body>
</html>
```

### Step 3: Start Tomcat

Start Apache Tomcat by executing the appropriate startup script in the `bin` directory:

- On Windows: Run `startup.bat`.
- On Unix-based systems: Run `startup.sh`.

### Step 4: Access the JSP File

Open your web browser and navigate to `http://localhost:8080/mywebapp/hello.jsp`. You should see the "Hello, Apache Tomcat and JSP!" message.

### Step 5: Stop Tomcat

When you're done, you can stop Tomcat by executing the appropriate shutdown script in the `bin` directory:

- On Windows: Run `shutdown.bat`.
- On Unix-based systems: Run `shutdown.sh`.

