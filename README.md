# Eventstream
Event Stream using Fabric

ETL Process for a real-time data using Eventstream
1. Configure Python script to stream data using Event Hub protocol
![alt text](image.png) 

2. Run the script to start streaming
![alt text](image-1.png)

3. Some rows have more than one reading coming from different censors
![alt text](image-2.png)

4. Add Expand transformation to make sure reading from each censor falls on a single row
![alt text](image-3.png)

No more arrays in temperature readings column
![alt text](image-4.png)

5. Add manage fields to select and transform columns
![alt text](image-5.png)

![alt text](image-6.png)

![alt text](image-7.png)

Data after transformation
![alt text](image-9.png)

6. Calculate average temperature by event id using group by
![alt text](image-8.png)

Average temperature by event id
![alt text](image-10.png)

7. Join average temp with original table using Join transformation
![alt text](image-18.png)

Joined tables
![alt text](image-11.png)

8. Select and Rename columns using manage transformation
![alt text](image-13.png)

![alt text](image-14.png)

9. Configure Destination for transformed data and Publish Eventstream so it starts to ingest data
![alt text](image-15.png)

10. Live Eventstream
![alt text](image-16.png)

11. Data in Eventhouse
![alt text](image-17.png)