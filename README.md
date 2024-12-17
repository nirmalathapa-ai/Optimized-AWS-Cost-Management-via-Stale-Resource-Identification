# Optimized-AWS-Cost-Management-via-Stale-Resource-Identification
This project features a Smart AWS Lambda Function that optimizes storage costs by identifying and deleting unused snapshots. The function scans snapshots and checks for links to active EC2 instances. If no active instance is found, the snapshot is automatically deleted, ensuring efficient AWS cost management and resource optimization.




### Problem:  
Developers often create EC2 instances with attached volumes and take snapshots for backup purposes. However, when these EC2 instances are terminated, the associated snapshots are often forgotten and remain in storage. These unused snapshots continue to incur unnecessary costs, even though they are no longer needed.  

### Solution:  
To optimize AWS storage costs, we implemented an intelligent Lambda function. This function automatically scans all snapshots and checks for their association with active EC2 instances. If it detects snapshots that are not linked to any active EC2 instances, it deletes them. This automated process ensures that unused snapshots are removed, helping to reduce unnecessary storage costs and improve AWS cost efficiency.
