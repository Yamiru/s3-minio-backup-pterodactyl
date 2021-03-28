# TUTORIAL MINIO S3 STORAGE BACKUP


MINIO S3 STORAGE BACKUP INSTALL PTERODACTYL:

(game/voice/.. server backup to another server)

1.	Download egg https://github.com/parkervcp/eggs/tree/master/storage/minio
2.	Upload S3 egg to pterodactyl panel
3.	Install wings /external server(vps/vds/ds)  and add to Panel NODES
4.	Install S3 Storage server with custom defined port –wait for server ready /green/
5.	normal/update/rotate to normal - startup type(pterodactyl - manage server)
6.	copy filemanager – keys key&secret
7.	login http://7.9.109.124:26611 and create bucket (name: first) --> edit policy to read/write
8.	edit panel side file .env and add this to end (with yours data):

```
# Set your panel to use s3 for backups
APP_BACKUP_DRIVER=s3

# Info to actually use s3
AWS_DEFAULT_REGION=us-east-1
AWS_ACCESS_KEY_ID=7n4WTXSfFwLNEDDln1ekbDTrbZ6YWsMcKH
AWS_SECRET_ACCESS_KEY=XLmSSD6P3dDNVYB5GwPOvjaXpcBhQYzIBU

# Name of the bucket that you created
AWS_BACKUPS_BUCKET=first

# Only required if you're not using AWS
AWS_ENDPOINT=http://7.9.109.124:26611
```

9.	save and restart panel if not work try https://pterodactyl.io/panel/1.0/updating.html
10.	done :D

Thank you/Ďakujem and follow me 😊
