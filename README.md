**DKJmeterLoadAndAPITesting**
				
 **Now, let’s see the process of performing JMeter API testing.**

 Demo: JMeter API Testing

To download JMeter, you will need to access the Apache JMeter website and download the file.

The first step is to set up the Apache JMeter, as shown below.

**•	Go to the Apache JMeter folder → bin folder → open the batch file.**

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

**Now, try one more thing:**

•	Go to the thread group
 
•	Change the number of threads to be 10

•	Run the test

After running the test, check the "results in the table" and see the testing being performed. This can be seen in case "view results in the table" is available too.

In the view results tree, you can click on a request and see different information. Here you can see the sample start, load time, latency error, etc. In the "view results in table," window, you will be able to see all the information in a tabular format.

![image](https://user-images.githubusercontent.com/117725893/219645416-e2af0246-6958-4049-817f-5f7d18f0801f.png)

You can also see the response data in the above image. This is the same data available when you copied the URL from the browser. Furthermore, the response headers and the request placed can also be checked
![image](https://user-images.githubusercontent.com/117725893/219645517-7a836aa8-e3fe-4d2a-9db4-dd069818a5fe.png)









**Now, let’s see the process of performing JMeter Website testing.**

Demo: JMeter Website Testing

**•	Create Jmeter test**

In the left side you can see the elements of the test plan. 
![image](https://user-images.githubusercontent.com/117725893/225824259-4abcbf15-b109-4022-8c49-bcb59a9c8c37.png)    
------------------------------------------------------------------ Test Plan and Configurations of them ----------------------------------------------
**Test plan contains all the elements that is need to perform your test.**

You can provide any name to your Jmeter Test [First].
![image](https://user-images.githubusercontent.com/117725893/225824415-6c5821bd-c6c0-4c09-915c-cecb2f34b0ea.png)    
------------------------------------------------------------------ Test Plan Name : First --------------------------------------------------------------


If you right click your Test Plan and go to Add, you can see various elements under a drop down list.
![image](https://user-images.githubusercontent.com/117725893/225824521-359aa422-72fc-433c-9c3f-216539233584.png)    
------------------------------------------------------------------ Test Plan > Add > Various Elements ----------------------------------------------


The first thing that you need to add  a Thread Group.
![image](https://user-images.githubusercontent.com/117725893/225824649-774a4bcb-e275-45c2-975e-ac4039f3fac3.png)    
------------------------------------------------------------------ Add > Thread Group ---------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225824760-6d94da90-4b82-4c28-866c-8e577bcd261d.png)    
------------------------------------------------------------------ Thread Group ----------------------------------------------------------------------


**Thread Group is the number of users who will be used to create or run the test.**

I have named my Thread Group as Number of User.
![image](https://user-images.githubusercontent.com/117725893/225824867-50992b82-4c7d-4206-9550-cf2a32b49bca.png)    
------------------------------------------------------------------ Thread Group > Number of User --------------------------------------------------

**Let’s see some of the options under the Thread Group :**

**(i). Action to be taken after a sampler error: In case of any error what test should do, should it continue, start next thread loop,stop thread,stop test or to stop test now.**

**(ii). Thread Properties:**

•	Number of Threads (Users): Number of users that you will use to test

•	Ramp-Up period(in seconds) : How long to delay between starting each user/thread

•	Loop count : The loop count, run forever or particular number of loops

•	Delay Thread creation until needed: If you want to delay the thread

•	Scheduler: Schedule the test case for a particular time

Right click on the Thread Group or the Number of User, go to Add and add Sampler to add a request. see all the kind of requests that Jmeter supports.
![image](https://user-images.githubusercontent.com/117725893/225825528-605f9a1e-09c7-4a6e-839a-38826668f02f.png)    
------------------------------------------------------------------ Sampler Section --------------------------------------------------------------------


let’s take a HTTP Request.
![image](https://user-images.githubusercontent.com/117725893/225825914-6648d7cf-9355-4d35-9bfb-994906430011.png)    
------------------------------------------------------------------ HTTP Request ----------------------------------------------------------------------- 


**You can rename your HTTP request.**

•	Server or the IP - copy and paste the web site url that you are going to test. When pasting the url “Enter Website URL”, you need not to provide the “https://” protocol section and the forward slash which is available at the end of the url as well.

•	Port number — enter the port number.

If you want to move to another page in your web site, you need to insert that path in the Path text box.
“/all/course”
![image](https://user-images.githubusercontent.com/117725893/225826095-ec350e4e-5c12-4db1-9b28-ede88c5d448b.png)    
------------------------------------------------------------------ HTTP Request ----------------------------------------------------------------------


HTTP request is ready, but before running the test case we need to add some more elements to verify the result. we can add some listeners.

I have selected View Results in Table and View Results in Tree listeners.
![image](https://user-images.githubusercontent.com/117725893/225826515-5012c262-c6e1-4622-8dc4-9c5487f55da3.png)    
------------------------------------------------------------------ View Results in Table ---------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225826625-5f3d72a3-13ac-4fdd-b109-bb13ab09f62a.png)    
------------------------------------------------------------------ View Results in Tree ----------------------------------------------------------------


**Let us see how the result will look like with the result tree and the result table.**

**To run test there are several options.**

1.	Go to Users right click and select Start.
![image](https://user-images.githubusercontent.com/117725893/225826756-4b390b57-8f8a-49d3-b834-fa9f7b859049.png)    
----------------------------------------------------------------- Number of User > Start ------------------------------------------------------------
2. Go to Run in the menu bar and click Start.
![image](https://user-images.githubusercontent.com/117725893/225826859-4fc07e90-e3d5-4ed6-8739-c03130114f44.png)    
------------------------------------------------------------------ Run > Start -------------------------------------------------------------------------
3. Click on Star button.
![image](https://user-images.githubusercontent.com/117725893/225826946-a1dbc478-add1-40f4-aa69-28ec7a2ecb05.png)    
------------------------------------------------------------------ Click on the start button -----------------------------------------------------------
After clicking start, you can see a dialog box asking you to save your test case. You should save your test case, if you are reusing the same test case.
![image](https://user-images.githubusercontent.com/117725893/225827087-496dedac-7797-4fbd-8a51-c66b4a5e8d7c.png)    
------------------------------------------------------------------ Save the Test Case ------------------------------------------------------------------ 


**It has already executed, if you go to the results :**

•	 “HomePage” has executed with a Sample Time(ms) 3127 ms (time that web page took this request to execute).

•	The Status is green, so that means this test case has successfully executed.
![image](https://user-images.githubusercontent.com/117725893/225827179-b68c66f9-4861-4e33-b2d1-2d6233bb6f81.png)    
------------------------------------------------------------------ Results in a Table ------------------------------------------------------------------

View Results Tree: see the results.
![image](https://user-images.githubusercontent.com/117725893/225827343-e8ce9222-5876-4150-a43f-b8f87753fcca.png)    
------------------------------------------------------------------ Results in Tree --------------------------------------------------------------------- 

![image](https://user-images.githubusercontent.com/117725893/225827675-f8990735-6eb2-44d5-9ebf-ed82f73f042d.png)    
------------------------------------------------------------------ Results in Tree :Request ------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225827734-747c828d-8a47-4c93-9c69-8b2cec702777.png)    
------------------------------------------------------------------ Results in Tree :Response Data ----------------------------------------------------


You could not see any detail related to above test since the test executed very fast for a single thread/user. If you want to go through more details, increase the Number of Threads (Users). Also you can increase the Ramp-Up Period.In my test case ramp up period is 20 seconds.

Number of threads:10 and Ramp-up Period:20 seconds: for every two seconds one user will be added, within 20 seconds 10 users will be added.

If you click Loop Count as forever, the test will keep running until you forcefully stop it or you can uncheck forever check box and provide some loop count.
![image](https://user-images.githubusercontent.com/117725893/225827856-170f1b55-c296-4c6c-8b1b-d5577a9a0461.png)    
------------------------------------------------------------------ Number of User Configurations ---------------------------------------------------

If you want to clear the test results you can click on the button Clear All/Clear button.
![image](https://user-images.githubusercontent.com/117725893/225827956-1561797a-331c-4abf-96d5-ffb9365cc9c6.png)    
------------------------------------------------------------------ Clear the Test Results --------------------------------------------------------------

You run your test case you can see number of users who hit the web site in the right top corner (5/10) and a green color button until your test case continue to run.
![image](https://user-images.githubusercontent.com/117725893/225828144-e5fe7069-92e3-421e-99b0-cc1c6a02fd75.png)        
------------------------------------------------------------------ 5 Users Out of 10 (5/10) ------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225828241-ae73480e-99f9-4298-9ff7-b9cb706db204.png)              
------------------------------------------------------------------ 10 Users (10/10) --------------------------------------------------------------------

To stop the test case you have stop button and shut down button.
![image](https://user-images.githubusercontent.com/117725893/225828323-554f7f62-4972-4d09-8490-e17ae8bc9c86.png)    
------------------------------------------------------------------ Stop/Shut down button ------------------------------------------------------------

**Assertions**

Assertion = Check on the response

Send your request to the server, you will get a response.If you want to do some checks on the response like whether you have receive the correct response code or you want to check some text in the response code or to test the format of the response all these checks will come under assertions

**Response Assertion**

Add an assertion, go to your Thread Group, Right click your Thread Group,go to Assertions and click on Response Assertions.
You can apply an assertion to the Main sample and sub samples, Main sample only,Sub-samples only or apply to Jmeter variable.

The next field in the Response Assertion window is the Field to Test. I have clicked Response Code as the field to test my response. Also you can test Text Response, Document (text),URL sampled and so on.

Check whether the response code is Equals 200, so for that we can write the code in the Patterns to Test text box. This assertion will check the response code and compare with 200, if this matches it will pass the test case or if not it fail.

You can change the pattern and see how assertion work to your project.
![image](https://user-images.githubusercontent.com/117725893/225842877-e2bf1887-cf97-460b-b33a-205e3ced5e4f.png)    
------------------------------------------------------------------ Response Assertion ----------------------------------------------------------------

Results have generated here,and every detail is in green that means test case has passed.We can cross verify it by going to the result tree and we can see response code as 200 and every response is giving 200. That means assertion has passed.
![image](https://user-images.githubusercontent.com/117725893/225843010-195faa5e-20b2-4669-bd6c-b9ef58d2baca.png)    
------------------------------------------------------------------ Results in Table --------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225843096-b99fc9d0-d742-44c5-b6bd-6936012dddc0.png)    
------------------------------------------------------------------ Response code : 200 (Results in Tree) ----------------------------------------------

Changed my response code to 202.
![image](https://user-images.githubusercontent.com/117725893/225843235-0931ff77-5be2-4100-a333-13c743a45280.png)    
------------------------------------------------------------------ Changed the response code to 202 -----------------------------------------------

The test should fail because the server is giving back the response 200 but I am expecting 202 as the response code. The status is in red color.
![image](https://user-images.githubusercontent.com/117725893/225843373-bb41eb9a-9324-4468-8ab0-8baa5a7200ec.png)    
------------------------------------------------------------------ Result in Table ---------------------------------------------------------------------

If I expand the text in response from the tree, it show Response Assertion failure and it is clearly telling us that we expected 202 but we received 200. So that is why it is a failure.
![image](https://user-images.githubusercontent.com/117725893/225843514-5f383c38-e9ef-4615-951e-fb5eea454b6d.png)    
------------------------------------------------------------------ Results in Tree ---------------------------------------------------------------------

To get a better view of the assertions, add a new listener Assertion Results.
![image](https://user-images.githubusercontent.com/117725893/225843641-e6173771-b73b-486d-98f2-2b460e7207ad.png)    
------------------------------------------------------------------ Add > Listeners > Assertion Results -----------------------------------------------

Run the test case and see how Assertion Results display.Every time when assertion fail, a result is logged here we can observe the failure.
![image](https://user-images.githubusercontent.com/117725893/225843745-d5883ce5-c330-4f85-95ab-b5541a480bfd.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------

**Comparison is 202 and received 200.**

When Run the test case again with the correct response code 200.

In the assertion results, don't display any exception. Status is in green where everything successfully executed.
![image](https://user-images.githubusercontent.com/117725893/225843880-6df1b7b8-104f-4051-bdd7-20b75b74b2b5.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225843955-a485bfbd-ea48-4bf8-843d-78fd4dca104b.png)    
------------------------------------------------------------------ View results in Result Tree ---------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225844020-efab8860-c32c-44e6-9322-ecd69f20b929.png)    
------------------------------------------------------------------ View results in Result Table --------------------------------------------------------

**Duration Assertion**

Checking the duration of the response. We can apply it to Main sample and sub samples, Main sample only or Sub-samples only. I have added 2400 ms as the Duration. If the request takes more than 2400 ms will be a failure and will get notified in the Assertion Results.
![image](https://user-images.githubusercontent.com/117725893/225844158-7650f4d3-cc37-400f-8ea4-4684f7e70328.png)    
------------------------------------------------------------------ Duration Assertion -----------------------------------------------------------------

Run the test case and see how duration assertion work.My test results. Test results only one request took more than 2400 ms.
Assertion Results
![image](https://user-images.githubusercontent.com/117725893/225844303-7c9ac3f3-de2a-44c1-a076-14f9ee249b7e.png)    
------------------------------------------------------------------ View Result Tree --------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225844365-d6fc62c4-2846-4e43-afe0-071876ac7010.png)    
------------------------------------------------------------------ Duration Assertion Failed -----------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225844435-69f36fcd-6eb3-4e07-8fbd-35f28e23662e.png)    
------------------------------------------------------------------ View Result in Table ----------------------------------------------------------------

**Size Assertion**

As name indicates it is related to the response size. I have added Size in byte as 41300 and I have added Type of comparison as equal sign (=).

If the request is equal to 41300, then it should pass else it should fail. Also you can use multiple comparisons available under Type of comparison.

My results you can see all size assertions are failed.
![image](https://user-images.githubusercontent.com/117725893/225844585-e44043f9-c987-4fff-990e-88624f2547f3.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225844675-d1dcb91c-19ec-47ad-bca3-25ad92fa7d75.png)    
------------------------------------------------------------------ View Results Tree -------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225844749-83825d20-9d42-4862-a699-25313bf34c30.png)    
------------------------------------------------------------------ View Results in Table ---------------------------------------------------------------

I changed the Type of Comparison in to greater than sign (>), all my test cases have passed.
![image](https://user-images.githubusercontent.com/117725893/225844872-1b3d1741-dd10-4043-b341-8f899254fb6e.png)    
------------------------------------------------------------------ Size Assertion ----------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225844950-fd52eedf-9f2c-4a73-8421-ac43197c97a4.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225845058-df0e39e3-cf62-4a03-a2f7-206e448661ad.png)    
------------------------------------------------------------------ View Result Tree --------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225845125-9c8b36bb-2fbc-4790-a224-d0cd674ce0c8.png)    
------------------------------------------------------------------ View Results in Table ---------------------------------------------------------------

**HTML Assertion**

Test the format of the response. It checks whether the format is valid HTML or not.If it is not a valid HTML it will throw some errors and fail the assertion.
![image](https://user-images.githubusercontent.com/117725893/225845241-178e1d3d-0276-4890-a14a-ed51ab73b572.png)    
------------------------------------------------------------------ HTML Assertion --------------------------------------------------------------------

See the result of the HTML Assertion,

Here you can see 0 error and 79 warnings.
![image](https://user-images.githubusercontent.com/117725893/225845362-0c70f799-897b-4482-b96c-f35cc0973439.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------
![image](https://user-images.githubusercontent.com/117725893/225845418-2768890f-3dd6-4cf8-9a23-9afc7632bef1.png)    
------------------------------------------------------------------ View Result Tree -------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225845471-14600c6b-9dc9-48b2-a960-6e5fbc61da41.png)    
------------------------------------------------------------------ View Results in Table ---------------------------------------------------------------

In HTML Assertion, you can provide Error threshold and Warning threshold. In my case, Error threshold is 3 and Warning threshold is 79.
![image](https://user-images.githubusercontent.com/117725893/225845579-477e8977-35f7-4935-afc4-22f4f0a7d088.png)    
------------------------------------------------------------------ Error threshold and Warning threshold -------------------------------------------

If there are errors more than 3, it should fail.
![image](https://user-images.githubusercontent.com/117725893/225845684-6816ad52-e101-4f84-9104-21fdcb7a0c2b.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------

This time it didn’t fail because I have set a threshold to 3 errors and warnings to 79.

Even this provide the number of error and number of warning, we exactly don’t know the places/element which those errors occurred. To get report on that we can write that report to a file. You can browse and select a file to store all the errors. You can tick the box Errors only to store only the errors in the file.
![image](https://user-images.githubusercontent.com/117725893/225845836-be57da3f-c0e0-4566-80cb-8a56459755f3.png)    
------------------------------------------------------------------ HTML Assertion.txt File ------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225845900-6a940a6b-7fb2-4dbc-bfb2-72eba759fc19.png)    
------------------------------------------------------------------ HTML Assertion --------------------------------------------------------------------

You can see the file which provided all the errors.
![image](https://user-images.githubusercontent.com/117725893/225846024-3c7256cb-590c-4dab-838b-403f0805f1eb.png)    
------------------------------------------------------------------ HTML Assertion File ----------------------------------------------------------------

**You can do the test based on XML or XHTML as well.**

XML Assertion
![image](https://user-images.githubusercontent.com/117725893/225846259-a4f8e788-164c-455b-bcf8-469eeffc266e.png)    
------------------------------------------------------------------ XML Assertion ---------------------------------------------------------------------

This will check the format, if it is a valid XML it will pass otherwise it will fail.
![image](https://user-images.githubusercontent.com/117725893/225846383-8f214f82-01e3-4fb7-954c-76c1109bad14.png)    
------------------------------------------------------------------ XML Assertion ---------------------------------------------------------------------

XML Assertion failed and it says that the markup in the document preceding the an element type link must be followed by the ‘=’character.
![image](https://user-images.githubusercontent.com/117725893/225846499-28dd3704-3c0f-4cce-8ff0-bcb355cfc5bf.png)    
------------------------------------------------------------------ Assertion Result --------------------------------------------------------------------

Also you can write this Assertion to a file.
![image](https://user-images.githubusercontent.com/117725893/225846609-7d4b5a62-b42c-4b94-bf3d-f3d6895073f9.png)    
------------------------------------------------------------------ Assertion Results -------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/117725893/225846686-83fd39f7-476d-423b-985a-cebc931fc0b3.png)    
------------------------------------------------------------------ XML Assertion File ------------------------------------------------------------------



