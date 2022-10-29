# Info

This folder contains the generated HTML files. The MSL dataset exceeds the GitHub file size limit. Hence, it was moved to GitHub LFS. The direct link to the file can be obtained using the following CURL comand:

```
curl -X POST \
-H "Accept: application/vnd.git-lfs+json" \
-H "Content-type: application/json" \
-d '{"operation": "download", "transfer": ["basic"], "objects": [{"oid": "1d0a025e67ad8cdeb26ed0d38ce4be598b23ffa66cfe6c4a413c6a75fd08a936", "size": 121911104}]}' \
https://github.com/nfstream/SH-vs-ML.git/info/lfs/objects/batch
```

<!--- For more info on retreiving LFS files see:
https://gist.github.com/fkraeutli/66fa741d9a8c2a6a238a01d17ed0edc5
--->
