POST /v1/storage/buckets/{bucketId}/files HTTP/1.1
Host: cloud.appwrite.io
Content-Type: multipart/form-data; boundary="cec8e8123c05ba25"
X-Appwrite-Response-Format: 1.7.0
X-Appwrite-Project: <YOUR_PROJECT_ID>
X-Appwrite-Session: 
X-Appwrite-Key: <YOUR_API_KEY>
X-Appwrite-JWT: <YOUR_JWT>
Content-Length: *Length of your entity body in bytes*

--cec8e8123c05ba25
Content-Disposition: form-data; name="fileId"

"<FILE_ID>"

--cec8e8123c05ba25
Content-Disposition: form-data; name="file"

cf 94 84 24 8d c4 91 10 0f dc 54 26 6c 8e 4b bc 
e8 ee 55 94 29 e7 94 89 19 26 28 01 26 29 3f 16...

--cec8e8123c05ba25
Content-Disposition: form-data; name="permissions[]"

["read(\"any\")"]

--cec8e8123c05ba25--
