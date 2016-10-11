# Package a JAR containing your application
mvn package

# Check the created file
ls -la target/

# Use spark-submit to run your application
spark-submit --class "quickstart.spark.simple.SimpleApp" --master spark://127.0.0.1:7077 target/simple-project-1.0.jar ./data/test.txt