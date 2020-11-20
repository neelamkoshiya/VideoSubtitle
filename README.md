# VideoSubtitle
Learn how to transcribe video, translate  to multiple language and save it as a SRT file

Here is the high level architecture. Even though I have elaborated the process in Sagemaker Jupyter notebook. In reality you can put it on any compute and schedule it using Cloudwatch.

![Architecture diagram](https://github.com/neelamkoshiya/VideoSubtitle/blob/main/VideoSubtitles.jpg)

Steps:

1) Create sagemaker notebook : [create a notebook](https://docs.aws.amazon.com/sagemaker/latest/dg/howitworks-create-ws.html)
2) Make sure the sagemaker role has the right to use Transcribe, Translate and S3 bucket
3) Create S3 bucket: [create S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-bucket.html)
4) Load the mp4 file in the S3 bucket and reference the file location in your code.
