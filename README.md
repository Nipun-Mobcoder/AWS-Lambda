# AWS-Lambda
** AWS Lambda **  are serverless compute functions are fully managed by AWS where developers can run there code without worrying about servers. AWS Lambda function will allow you to run the code without provisioning or managing servers.

# Steps to Create an AWS Lambda Function

## a. Navigate to AWS Lambda
1. Log in to the AWS Management Console.
2. Search for **Lambda** in the AWS Services search bar and select it.

## b. Create a Function
1. Click **Create function**.
2. Choose a creation method:
   - **Author from scratch**: Start fresh with a custom function.
   - **Use a blueprint**: Use pre-built templates.
   - **Deploy a container image**: Use Docker images.

## c. Configure the Function
1. **Function Name**: Enter a unique name for your function (e.g., `myLambdaFunction`).
2. **Runtime**: Select the desired runtime (e.g., Node.js, Python, or Java).
3. **Permissions**: Assign an existing role or create a new role with basic Lambda permissions.

## d. Write the Code
1. In the **Code source** section, upload your code:
   - Use the inline code editor.
   - Upload a `.zip` file containing your code.
   - Reference an S3 location.
2. Example inline code for Node.js runtime:
   ```javascript
   exports.handler = async (event) => {
       return {
           statusCode: 200,
           body: JSON.stringify('Hello from Lambda!'),
       };
   };
   ```

## e. Deploy the Function
1. Click **Deploy** to save your changes.
2. Test the function by creating a test event and invoking it.

# Amazon API Gateway
** Amazon API Gateway ** is an AWS service for <mark style="background-color: lightblue"> creating, publishing, maintaining monitoring and securing REST, HTTP and websocket API's </mark> at any scale.
