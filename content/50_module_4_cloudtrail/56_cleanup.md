---
title: "Cleanup"
chapter: false
weight: 56
---

1. Delete the log group created to test the Falco rule modification

    ```
    aws logs delete-log-group --log-group-name "test_unused_region" --region="us-west-2"
    ```

1. Delete an S3 bucket

    ```
    aws s3api delete-bucket --bucket $BUCKETNAME
    ```

1. Remove CloudConnector Integration

    ```
    aws cloudformation delete-stack --stack-name CloudConnector
    ```
