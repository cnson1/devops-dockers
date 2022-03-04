# Exercsise:
![image](https://user-images.githubusercontent.com/94816681/156711308-f26d2641-0e62-46de-9bdc-eaeb1787a6db.png)

# Step to complete:
- Change inside Dockerfile
```
FROM ubuntu:20.04
WORKDIR /usr/src/app
COPY image-script.sh .
RUN apt-get update
RUN apt-get install -y curl
RUN chmod +x image-script.sh
CMD ./image-script.sh
```
- insert `image-script.sh`
`echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;`


# My result:
![image](https://user-images.githubusercontent.com/94816681/156711258-ff091357-262d-4133-8bd2-9e5a75a95170.png)
