DKJmeterLoadAndAPITesting

Now, let’s see the process of performing JMeter API testing.

Demo: JMeter API Testing

To download JMeter, you will need to access the Apache JMeter website and download the file. 

The first step is to set up the Apache JMeter, as shown below.

•	Go to the Apache JMeter folder → bin folder → open the batch file.

![image](https://user-images.githubusercontent.com/117725893/219641827-da427048-6de5-4e95-9666-52876f2a7241.png)

This might take a while. Wait till the JMeter window opens on the screen.

It divides the home window into two sections: the left side has all the test plan elements, and on the right side, all the configurations of that element are added.
 
As you are on the test plan element, you can see the configurations of the same.

•	Right-click on the test plan

•	Select the add option

•	Then in the menu that appears, select the threads option and then thread groups

Here, the number of threads refers to the number of users. The ramp-up period in seconds option states the time gap between the users' hits. There is a loop count where you can choose how many times the test will run for the number of users, and also, you can select the test to run infinite times. 

There is also a scheduler here to help you schedule the test start-time and end-time.

![image](https://user-images.githubusercontent.com/117725893/219642942-b7b2326e-f138-4e1a-9bb2-82a9b537b01e.png)

•	Identify the URL for this API

•	Copy this URL and open the JMeter window

Then in the JMeter window, do the following:

•	 Right-click on the Thread group

•	Navigate to “add”

•	In the box that appears, select “samplers”

You can see the types of requests that JMeter can work on

•	Choose the HTTP request. 

Here, you will have to give the address to some home pages or websites

•	In the Server Name or IP box, give the paste the GET API request URL 

•	In the Protocol box, put "HTTPS"

•	Now, put the path from the URL in the path box

•	Add the name in the parameters
![image](https://user-images.githubusercontent.com/117725893/219643650-24f1c024-99f0-48b3-b8d7-5eff988f517d.png)

After this HTTP request is ready, perform the test on it. To determine what the results of the test will be, add some listeners.

•	Right-click on the Thread group

•	Go to listener options

•	In the box, check the different types of reports that JMeter provides

•	For now, Select two "view results tree" and “view results in table"

•	Then save the test and run it

Simply click on the green button to run the test.

After running the test, it's time to check the results:

•	Go to the "view results tree"

The green status shows that the test was successful.
 
•	Then go “view results in a table”

The green status again shows the test was successful.
 
Since the number of threads and loop was denoted as one - both at the entry in both the results, the test result has come out accordingly.

Now, try one more thing:

•	Go to the thread group
 
•	Change the number of threads to be 10

•	Run the test

After running the test, check the "results in the table" and see the testing being performed. This can be seen in case "view results in the table" is available too.

In the view results tree, you can click on a request and see different information. Here you can see the sample start, load time, latency error, etc. In the "view results in table," window, you will be able to see all the information in a tabular format.

![image](https://user-images.githubusercontent.com/117725893/219645416-e2af0246-6958-4049-817f-5f7d18f0801f.png)

You can also see the response data in the above image. This is the same data available when you copied the URL from the browser. Furthermore, the response headers and the request placed can also be checked
![image](https://user-images.githubusercontent.com/117725893/219645517-7a836aa8-e3fe-4d2a-9db4-dd069818a5fe.png)

