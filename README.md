# Fivetran
Using Fivetran to connect Google Sheets data to Google BigQuery and then to Looker for Visualization 

Step 1:
Set up a new Fivetran connection. Choose your source data. For this demo, we are using Google Sheets. 
![image](https://user-images.githubusercontent.com/68393151/230478246-f90c8227-f9f7-473a-9945-dadf7f0bdb68.png)

Step 2:
Choose your destination schema, table, and your authentication method. It's recommended that you use 'Authorize Service Account' as this will allow you to limit access to only certain spreadsheets. 

Step 3:
In your google shreadsheet, you need to select the data you want to use, and create a named range under the Data tab at the top. 
![image](https://user-images.githubusercontent.com/68393151/230482224-28af070b-6d58-4ee6-a78b-62f333842ff3.png)

Step 4:
Next you'll need to share said spreadsheet with the given email address, and then share the URL of the shreadsheet. Next select find sheet, to find your spreadsheet. Third, select the named range you created in step 3. Edit the data processing location and cloud service provider if needed. Then select 'Save and Test'
![image](https://user-images.githubusercontent.com/68393151/230482445-b33900ae-574b-4297-b56d-c0bcd7d59f04.png)

Step 5:
If the prior steps were completed, you should see that your connection tests were sucessful. 
![image](https://user-images.githubusercontent.com/68393151/230483031-79f8566b-7880-45a5-a688-5e9d6c44bcb8.png)

Step 6:
Next up, we will choose the destination for our data. There are quite a few options, so make sure you choose the correct one. For this example we are going to use Google BigQuery. 
![image](https://user-images.githubusercontent.com/68393151/230484503-61269682-fdc5-489a-8441-a2459f4598c7.png)

Step 7: 
On the next page, make sure your destination information is correct. This will vary from system to system, but with some tweaks you should be moving data in not time. 
![image](https://user-images.githubusercontent.com/68393151/230485105-0aa1f728-971f-492a-8ee3-57c52787d501.png)

Step 8:
Next up is a cool feature. You can choose to protect sensitive data through a hashing system or a block, so that you can protect SSN, CC, or PII info in your data. 

Step 9:
'What are you syncing about?' Your data should be connected at this point. You can start syncing your data now or later, depending on your needs. 

Step 10: 
Once your data has synced, you should be able to choose the frequency of the sync, and monitor sucessful syncs. You can also choose to transform your data at this point. Fivetran has great built in tools to transform your connected data. At this point, we are going to connect this data to a BI tool for analysis. 
![image](https://user-images.githubusercontent.com/68393151/230487554-fc314b00-d7dd-4f81-888b-ed85d95985a1.png)

Step 11:
Let's connect this data to Google Data Studio aka Looker. After connecting to your BI tool, select 'View BI Tool' at the bottom. 
![image](https://user-images.githubusercontent.com/68393151/230489338-da104798-9de9-4a23-a975-d7d374f64235.png)

Step 12:
To view this data, we need to open Looker. Sign in as needed, and open a new dashboard/report. In Looker, you can then select BigQuery, and connect to the data source we just made in Fivetran. Make sure to select your correct project, dataset, and table. 
![image](https://user-images.githubusercontent.com/68393151/230490084-0e5729ee-3e61-4bb8-8adb-c6ba408b7fe4.png)

Step 13:
Start visualizing! From here on out you should be able to create any dashboards and reports you want, and Fivetran will keep the pipeline flowing at your specified interval. 
![image](https://user-images.githubusercontent.com/68393151/230624012-6a1a903b-f4f0-450d-b18c-d04d11dac374.png)

![image](https://user-images.githubusercontent.com/68393151/230624090-5083c905-67f8-4598-9111-c91af7686f72.png)

