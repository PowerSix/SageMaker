### Prerequisites
1. Create an [Amazon SageMaker Notebook instance](https://docs.aws.amazon.com/en_pv/sagemaker/latest/dg/howitworks-create-ws.html) and copy the whole repository to it. Notebook should have an IAM Role with permission to AWS AI Service (Rekognition, Polly, Transcribe, Translate, Comprehend, Comprehend Medical. etc.)
2. Lauch [Media Analysis Solution](https://aws.amazon.com/solutions/media-analysis-solution/) by deploying the CloudFormation stack.
3. Launch [Amazon Transcribe Websocket Static](https://github.com/aws-samples/amazon-transcribe-websocket-static) by deploying to Amplify Console.
4. Create an IAM user to use with Transcribe only with the policy defined in this [policy.json](https://github.com/aws-samples/amazon-transcribe-websocket-static/blob/master/policy.json).

### 1 - AWS AI Services Demo Notebook:
In this demo, you will demonstrate the capabilities of Amazon Rekognition, Amazon Polly, Amazon Comprehend, Amazon Translate and Amazon Transcribe.

### 2 - Textract
In this demo, CV.png will be used to demonstrate how Textract can help to analyze a document to extract key-value pairs and tables with it's dependencies.

### 3 - Comprehend

#### ComprehendCustom Notebook
Amazon Comprehend provides the capability to create custom classifier. In this notebook we will use AG News data set to create a custom classifier and then get the realtime news feed from BBC as a test dataset. Start a classification job using the trained custom classifier and validate how the news articles are getting classified.

#### ComprehendMedicalDemo notebook
In this demo, we will use Rekongition to identiy text in a chest x-ray and use Comprehend Medical to identify Personal Health Information (PHI) in the detected text and mask it.

### 4 - Translate
Amazon Translate supports providing custom terminologies so that you can translate a specific content in the way that you want. In this demo, we use a custom_terminologies.csv file to create a custom terminology and validate how it performs.