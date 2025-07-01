# IoT Core to Kinesis Firehose to S3 Pipeline

Ingest IoT data via AWS IoT Core, stream it through Kinesis Firehose, store it in S3 as Parquet files with dynamic partitioning, and query it using Glue.

# Deployment

Change parameter values in `samconfig.toml`.

```bash
sam deploy
```

## License

[MIT License](LICENSE)
