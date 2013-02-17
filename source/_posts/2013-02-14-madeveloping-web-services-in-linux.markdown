---
layout: post
title: "Developing Web Services in Linux"
date: 2013-02-14 17:40
comments: true
categories: [web services,netbeans,linux,ubuntu,joss,programs,programming,java]
---
**Web services** enable software components such as application functions, objects and processes from heterogeneous systems to be exposed as services over the Internet.

To develop Web Services on Linux, we need the following packages.

**1.Java SE Development Kit (JDK)**

**2.NetBeans IDE**

To install these packages, follow the below steps :-

First install Java SE Development Kit

To install proprietary Java, you must have the Multiverse repository enabled. Click on *System* > *Administration* > *Software Source* > *Select Multiverse* Close.

When ask to reload the package informations, Click *Reload*.

Open a terminal and type the following command :-

`sudo apt-get install sun-java6-jdk`

{% img center /images/ws16.png Developing Web Services in linux image1 %}

To setup the default java version

`sudo update-java-alternatives -s java-6-sun`

Next setup the environment variable

You also need to setup *JAVA_HOME* and *PATH* variable.Open your *.bash_profile* file:

`sudo gedit $HOME/.bashrc`

Append following line:

`export JAVA_HOME=/usr/lib/jvm/java-6-sun`

`export PATH=$PATH:$JAVA_HOME/bin`

Save and close the file.

Then download NetBeans IDE from *here*

Open a terminal and *cd* to the downloaded location.Then type

'sudo sh netbeans-6.7.1-ml-linux.sh'

{% img center /images/ws1.png Developing Web Services in linux image2 %}

Click *Next* and Accept the License.It will automatically detect JDK.Don’t change the default installation paths.

{% img center /images/ws3.png Developing Web Services in linux image3 %}

When the installation is complete, click *Finish* to exit the wizard.

Now we will develop our first web service using netbeans. For a change instead of developing a Hello Web Service as the first web service, we will develop a Calculator Web Service to add two integer numbers.

##Creating a Web Service

1.Choose *File > New Project (Ctrl-Shift-N)*. Select *Web Application* from the *Java Web* category.

{% img center /images/ws7.png Developing Web Services in linux image4 %}

2.Name the project *CalculatorWebService*.

{% img center /images/ws8.png Developing Web Services in linux image5 %}

3.Click through the remaining pages and click *Finish*.

{% img center /images/ws9.png Developing Web Services in linux image6 %}

4.Right-click the *CalculatorWebServic*e node and choose *New > Web Service*.

5.Name the web service *CalculatorWS*, type *org.me.calculator* in Package, and click *Finish*.

{% img center /images/ws10.png Developing Web Services in linux image7 %}

The Projects window displays the structure of the new web service and the source code is shown in the editor area.

{% img center /images/ws66.png Developing Web Services in linux image8 %}

6.Change to the *Design* view.

Click *Add* Operation in the visual designer. A dialog box appears where you can define the new operation.
In the upper part of the Add Operation dialog box, type *add* in Name and type *int* in the Return Type drop-down list. In the lower part of the Add Operation dialog box, click *Add* and create a parameter of type *int* named *i*.Then click *Add* again and create a parameter of type *int* called *j*.

{% img center /images/ws11.png Developing Web Services in linux image9 %}

Click *OK* at the bottom of the Add Operation dialog box.

The visual designer now displays the following:

{% img center /images/ws12.png Developing Web Services in linux image10 %}

7.Click *Source* and notice that the source code that has been generated in the previous steps is as follows:

8.In the editor, extend the skeleton add operation to the following (changes are in bold):

@WebMethod

public int add(@WebParam(name = “i”)

int i, @WebParam(name = “j”)

int j) {

**int k = i + j;**

return **k**;

}

{% img center /images/ws13.png Developing Web Services in linux image11 %}

9.Right-click the project and choose *Deploy*. The IDE starts the application server, builds the application, and deploys the application to the server.

You can follow the progress of these operations in the *CalculatorWSApplication (run-deploy) and GlassFish V3 Prelude* tabs in the *Output view*.If you deployed to the GlassFish V3 Prelude Server, you will see the following, which indicates that you have successfully deployed your web service:

{% img center /images/ws14.png Developing Web Services in linux image12 %}

##Consuming the Web Service

Now that you have deployed the web service, you need to create a client (jsp page) to make use of the web service’s add method.

In this section, we will create a new web application and then consume the web service in the default JSP page that the Web Application wizard creates.

1.Choose *File > New Project (Ctrl-Shift-N)*. Select *Web Application* from the *Java Web* category. Name the project *CalculatorWSJSPClient*. Click *Finish*.

2.Right-click the *CalculatorWSJSPClient* node and choose *New > Web Service Client*.

3.In *Project*, click *Browse*. Browse to the web service that you want to consume. When you have selected the web service, click *OK*.

{% img center /images/ws18.png Developing Web Services in linux image13 %}

4.Leave the other settings at default and click *Finish*. The Projects window displays the new web service client, as shown below:

{% img center /images/ws17.png Developing Web Services in linux image14 %}

5.In the Web Service References node, expand the node that represents the web service. The *add* operation, which you will invoke from the client, is now exposed.

6.Drag the add operation to the client’s index.jsp page, and drop it below the H1 tags. The code for invoking the service’s operation is now generated in the *index.jsp* page.

Change the value for *i* and *j* from *0* to other integers, such as *3* and *5*. Replace
the commented out TODO line in the catch block with *out.println(“exception” + ex);*.

<%

try {

org.me.calculator.CalculatorWSService service = new org.me.calculator.CalculatorWSService();

org.me.calculator.CalculatorWS port = service.getCalculatorWSPort();

// TODO initialize WS operation arguments here

int i = **3**;

int j = **5**;

// TODO process result here

int result = port.add(i, j);

out.println(“Result = “+result);

} catch (Exception ex) {

**out.println(“exception” + ex);**

}

%>


7.Right-click the project node and choose *Run*.The server starts, if it wasn’t running already. The application is built and deployed, and the browser opens, displaying the calculation result:

{% img center /images/ws15.png Developing Web Services in linux image15 %}

License
-

Paul S

*Free Software Supporter!*

*Tested in Ubuntu and JOSS Linux*




