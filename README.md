# aws-image-manage

manage image resources in amazon web services for a specific django project (https://data.tnris.org)

- iterate through aws s3 bucket and copy all related images with .jpg suffix
- copy to new image file with uuid as file name
- delete old images after copy has been made
- update postgres rds instance (two different tables) with new uuid image file url
