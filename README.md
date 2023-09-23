# MIMEAttachment_http_Boomi

![image](https://github.com/manasch19/MIMEAttachment_http_Boomi/assets/97012694/f6d6b0ee-b6c9-4d69-b6ba-7ce003678cc4)


Step 1 : Getting file from Disk
Step 2: setting MIME name

![image](https://github.com/manasch19/MIMEAttachment_http_Boomi/assets/97012694/037ee4aa-cea9-4bb1-8e59-6f359e115977)

Step 3: send the file to cache

![image](https://github.com/manasch19/MIMEAttachment_http_Boomi/assets/97012694/e8b75ae6-c122-422b-b4f1-7bd9a5d132f1)

Step 4:configure http resource path

Step 5: configure Request body
![image](https://github.com/manasch19/MIMEAttachment_http_Boomi/assets/97012694/c282768f-eb3d-40af-a0c0-43ee8aa3a299)

example: '{
      "file" : {
         "value" : "'{1}'",
         "Content-Type" : "application/octet-stream",
         "Content-Transfer-Encoding":"binary",
         "type" : "key"
      }
}'

Step 6: Use dataproces Map JSON to MIME function

![image](https://github.com/manasch19/MIMEAttachment_http_Boomi/assets/97012694/c362c9a4-8ce9-4cf0-b10d-755db54c6a87)


Step 7: Use Http connecter and send this as attachment

![image](https://github.com/manasch19/MIMEAttachment_http_Boomi/assets/97012694/19011035-5610-48dd-b00d-dcff4df6e655)

example: content type = multipart/form-data;boundary=testboundary

Step 2:
