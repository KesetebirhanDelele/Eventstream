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

5. 