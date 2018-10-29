# aws-image-manage

manage image resources in amazon web services for a specific django project (https://data.tnris.org)

- iterate through aws s3 bucket and copy all related images with .jpg suffix
- copy to new image file with uuid as file name
- delete old images after copy has been made
- update postgres rds instance (two different tables) with new uuid image file url

### requirements

- install [boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#installation) with `pip install boto3`
- install [pyscopg2](http://initd.org/psycopg/docs/install.html) with `pip install psycopg2`
- [uuid](https://docs.python.org/3/library/uuid.html) (included with standard library)
- [datetime](https://docs.python.org/3/library/datetime.html) (included with standard library)
- [os](https://docs.python.org/3/library/os.html) (included with standard library)
