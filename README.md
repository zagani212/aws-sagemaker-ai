# News aggregator

# Download dataset

we will work on uci new dataset that you can download from this link : https://archive.ics.uci.edu/dataset/359/news+aggregator

# Upload dataset to S3

After unzipping the dataset you should create an S3 bucket and upload your dataset file on it

![](./images/upload%20datatset.png)


# Amazon SageMaker AI

go and create your domain on Amazon SageMaker AI and select `set up for single user`

![](./images/sagemaker.png)


# Set Up IAM Role

Go to your domain and get your doamin'role name

![](./images/getRole.png)

then go to your IAM service, search for the execution role of your domain 

![](./images/search%20for%20role.png)

click on it and add an `AmazonS3ReadOnlyAccess`

![](./images/policies.png)

Before to start creating our jupyter file, you should chnage your instance type to one more powerful, for that go on Amazon sageMaker AI, select your domain 

il you don't already have one space create one by clicking on `JupyterLab` icon on top left, if you already have one click on it
![](./images/sagemaker%20studio.png)

Stop your instance, wait for it... and then upgrade instance type by choosing `ml.t3.2xlarge`

![](./images/upgrade%20instance.png)