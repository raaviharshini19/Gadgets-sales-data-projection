# Gadgets-sales-data-projection
# Project 2 - Gadget Sales Data Projection

##  Title
**Process & Analyse the Sales Data of Tech Gadgets in Near Real-Time**

---

##  Tech Stack
- **Python** → Custom scripts & Lambda functions  
- **DynamoDB** → Stores gadget sales transactions  
- **DynamoDB Streams** → Capture real-time changes  
- **Kinesis Streams** → Near real-time event streaming  
- **EventBridge Pipes** → Route events from DynamoDB → Kinesis → Lambda  
- **Kinesis Firehose** → Deliver streaming data into S3  
- **Amazon S3** → Storage for raw & curated sales data  
- **AWS Lambda** → Transformations & error handling  
- **Amazon Athena** → Query sales data from S3  

---

## Architecture Flow
Sales Data (DynamoDB)
→ DynamoDB Streams
→ EventBridge Pipe
→ Kinesis Data Stream
→ Lambda (Transform)
→ Kinesis Firehose
→ S3 (Data Lake)
→ Athena (Query & Analysis)
