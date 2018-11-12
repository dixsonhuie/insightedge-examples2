# insightedge-examples2


Example to submit uber jar on kubernetes
./insightedge-submit \
--master k8s://https://192.168.99.100:8443 \
--deploy-mode cluster \
--name SimpleIeApp \
--conf spark.kubernetes.authenticate.driver.serviceAccountName=spark \
--class com.samples.ie.SimpleIeApp \
--files https://raw.githubusercontent.com/dixsonhuie/insightedge-examples2/master/sample.txt \
--conf spark.kubernetes.container.image=gigaspaces/insightedge-enterprise:14.0.0-rc2 \
https://github.com/dixsonhuie/insightedge-examples2/raw/master/insightedge-examples2-1.0-SNAPSHOT-jar-with-dependencies.jar
