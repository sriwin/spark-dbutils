# Spark-Databricks Utils

## Databricks Command Line Login - Token Configuration

```
1. Execute
   pip install databricks-cli --upgrade
2. Execute
   databricks configure --token
3. it prompts for 			
	 Databricks Host: https://xxxxxxxx.net
	 Databricks Token: <<Create token in Databricks UI and paste it here>>
```

## Remove Folder

```
databricks fs rm -r dbfs:/xyx/stage/EventHub/Checkpoint-inbound-events/
```

## creates folders

```
databricks fs mkdirs dbfs:/xyz/stage/EventHub/Checkpoint-inbound-events/
```

## copies local files to databricks

```
databricks fs cp -r stage/Common/  dbfs:/xyz/Common/ --overwrite
```

## See the contents of the file
```
databricks cat dbfs:/xyz/pipeline1.json
```

## workspace 

```
databricks workspace import_dir . dbfs:/xyz/
databricks workspace mkdirs dbfs:/xyz/
databricks workspace ls /Users/someone@example.com/example -l
databricks workspace export "/Repos/someone@example.com/MyRepoNotebook" /Users/me/Downloads
databricks workspace import_dir -o Dfsc/xyz1 /xyz/abc
```
## List files in DBFS
```	
 dbfs ls dbfs:/xyz/
```

## uninstall
```
databricks libraries uninstall --all --cluster-id $clusterId
databricks clusters events --cluster-id $clusterId
databricks clusters start --cluster-id $clusterId
databricks clusters restart --cluster-id $clusterId
databricks libraries list --cluster-id $clusterId
```
