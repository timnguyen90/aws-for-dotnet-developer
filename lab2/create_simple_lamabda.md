# CREATE AND DEPLOY THE FIRST SIMPLE LAMBDA VIA THE VISUAL STUDIO.

> For the detailed of lambda function, please visit the link: https://docs.aws.amazon.com/lambda/latest/dg/welcome.html

## Step 1: Install the .NET CLI Templates for AWS
Please use the following command below to install:
`dotnet new -i Amazon.Lambda.Templates`

## Step 2: Install The AWS .NET Mock Lambda Test Tool
Please visit the page below for more information:
https://github.com/aws/aws-lambda-dotnet/blob/master/Tools/LambdaTestTool/README.md

## Step 3: Create the first lambda via Visual Studio

### Step 3.1:
From the Visual Studio IDE select `File => New => Project...`
![3.1](/lab2/images/lab2_0.png).

### Step 3.2:

![3.2](/lab2/images/lab2_1.png).

### Step 3.3:
![3.3](/lab2/images/lab2_2.png).

### Step 3.4:
![3.4](/lab2/images/lab2_3.png).

### Step 3.5:
![3.5](/lab2/images/lab2_4.png).

### Step 3.6:
From the Visual Studio, select the **Mock Lambda Test Tool** to run and test the lambda.

![3.6](/lab2/images/lab2_5.png).

### Step 3.7:
A new tab of your brower will be open, from the screen input your text, hit the button **Execute Function** to see the result.

![3.7](/lab2/images/lab2_6.png).

## Step 4: Deploy your very first simple Lambda to AWS.
*Before doing this step you have to make sure that, all the configurations from the **Lab1** is done*

### Step 4.1:
![3.8](/lab2/images/lab2_7.png).

### Step 4.2:
Select your: 
- **AWS Credentials:** `AWS credential on your local machine`
- **Region:** The region which you want to deploy on the AWS
- **Function Name:** the name of the lambda function which you want to display.

![3.9](/lab2/images/lab2_8.png).

### Step 4.3:
- **Role Name:** The role which you want to grant to your lambda function, in this case I select a default role which already created by AWS.
- **Memory:** The default memory capacity which you want to assign to the lambdafunction.
- ** DLQ Resource:** In case of failure, you wish the message want to sent the dead later queue or not.

![3.10](/lab2/images/lab2_9.png).

### Step 4.4:
After the uploading completed, a new screen will be appear to help you test your lambda on the AWS.
![3.11](/lab2/images/lab2_10.png).

### Step 4.5:
Go to the AWS Console, select the **Region** that you selected from **Step 4.2** then navigate to the Lambda service to check your lambda function.

![3.12](/lab2/images/lab2_11.png).