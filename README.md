# AWS S3

Upload or Sync large file or folder to AWS S3 Bucket

## Installation

Install AWS CLI [AWS CLI installation instructions](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) .

### Ubuntu
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

## Configure AWS CLI for S3

How to get AWS Account and Access Keys ? [AWS Account and Access Keys](https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html) .

### Setup Access key, Secret key & Region.

```bash
aws configure
```

### verify setting.
```bash
aws configure list
```

### List AWS S3 Bucket

```bash
aws s3 ls
```

## Command Upload or Sync large file or folder to AWS S3 Bucket

### Sync
```bash
aws s3 sync [Folder/file Path] s3://bucket-name/folder-name
```

Example
```bash
aws s3 sync /home/akshayrrao/Desktop/Backup s3://test-bucket/Backup
```

### Supported Commands in AWS S3
```bash
ls                                       | website                                 
cp                                       | mv                                      
rm                                       | sync                                    
mb                                       | rb                                      
presign
```
For more refer [S3](https://docs.aws.amazon.com/cli/latest/reference/s3/) .



## License
[MIT](https://github.com/Akshayrrao/Sync-large-file-or-folder-to-AWS-S3-Bucket/blob/main/LICENSE)
