# s3-bucket

프로젝트에서 사용할 S3 Bucket 을 생성합니다.

```bash
sam build
sam deploy --guided
```

고유한 S3 Bucket Name 을 이용하여 배포합니다.

```
Configuring SAM deploy
======================

	Looking for config file [samconfig.toml] :  Found
	Reading default arguments  :  Success

	Setting default arguments for 'sam deploy'
	=========================================
	Stack Name [your-stack-name]:
	AWS Region [ap-northeast-2]:
	Parameter BucketName [your-s3-bucket-name]:

...
```

S3 Bucket 의 Arn 및 고유값을 확인합니다.

```
CloudFormation outputs from deployed stack
-----------------------------------------------------------------------------------------
Outputs
-----------------------------------------------------------------------------------------
Key                 BucketUrl
Description         S3 Bucket Url
Value               http://<your-s3-bucket-name>.s3-website.ap-northeast-2.amazonaws.com

Key                 BucketRef
Description         S3 Bucket Ref
Value               <your-s3-bucket-name>
-----------------------------------------------------------------------------------------




CloudFormation outputs from deployed stack
-----------------------------------------------------------------------------------------
Outputs
-----------------------------------------------------------------------------------------
Key                 ResizedImageBucketRef
Description         S3 Bucket for Resized Image Ref
Value               your-bucket-resized

Key                 SrcBucketRef
Description         S3 Bucket for Src Image Ref
Value               your-bucket-src

Key                 ResizedImageBucketUrl
Description         S3 Bucket for Resized Image Url
Value               http://your-bucket-resized.s3-website.ap-northeast-2.amazonaws.com
-----------------------------------------------------------------------------------------
```
