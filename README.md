# IoT Core to Kinesis Firehose to S3 Pipeline

Ingest IoT data via AWS IoT Core, stream it through Kinesis Firehose, store it in S3 as Parquet files with dynamic partitioning, and query it using Glue.

```bash
sam deploy
```

Change parameter values in `samconfig.toml`.

## License

[MIT License](LICENSE)
