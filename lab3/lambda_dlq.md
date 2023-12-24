# [.NET] Using SQS dead-letter queues to replay messages.

## I. Diagram.

![3.1](/lab3/images/lab3_1.png)

## II. Detailed Steps.

### 1. Setup the SQS dead-letter queues.

**Step 1:** Create the sqs queue with the name  `ap-demo-main`.

![3.1](/lab3/images/lab3_2.png)

**Step 2:** Create the second sqs queue with the name `ap-demo-main-DLQ`.

![3.1](/lab3/images/lab3_3.png)

**Step 3:** Back to the queue `ap-demo-main`, go to the **Dead-letter queue**, Select the **Edit** button.

![3.1](/lab3/images/lab3_4.png)

**Step 4:** On the new screen, edit the configuration as the image.

![3.1](/lab3/images/lab3_5.png)


**Step 5:** Testing.

![3.1](/lab3/images/lab3_6.png)

![3.1](/lab3/images/lab3_7.png)

![3.1](/lab3/images/lab3_8.png)

![3.1](/lab3/images/lab3_9.png)


### 2. Buiding the AWS Lambda to process the message in teh dead-letter queue.

### 3. Testing.

### III. References.

- https://aws.amazon.com/blogs/compute/using-amazon-sqs-dead-letter-queues-to-replay-messages/