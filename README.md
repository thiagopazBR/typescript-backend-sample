# typescript-backend-sample


for dev
docker build --target=builder -t imagename:dev .


for production
docker build -t imagename .


# run
docker run -it \
-v log/:log/ \
-v /usr/share/zabbix/modules/files/content/:files/ \
hexing-azure-sql \
imagename
