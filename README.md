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

##
```
## removed folder
databricks fs rm -r dbfs:/xyx/stage/EventHub/Checkpoint-inbound-events/

## creates folders
databricks fs mkdirs dbfs:/xyz/stage/EventHub/Checkpoint-inbound-events/

## copies local files to databricks
databricks fs cp -r stage/Common/  dbfs:/xyz/Common/ --overwrite

```

