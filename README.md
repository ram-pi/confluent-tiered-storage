# Export AWS settings
```
export AWS_ACCESS_KEY_ID=<ACCESS_KEY>
export AWS_SECRET_ACCESS_KEY=<SECRET_KEY>
export BUCKET_NAME=<BUCKET_NAME>
export REGION=<REGION>
```

# Start docker-compose
`docker-compose up -d`

# Create sample data
`kafka-producer-perf-test --producer-props bootstrap.servers=localhost:19092 acks=all --topic test --num-records 300000 --throughput -1 --record-size 1000000 --print-metrics`

# Check on AWS for objects 
Naviage to Amazon S3 -> Buckets -> yourBucket and check for confluent objects.
