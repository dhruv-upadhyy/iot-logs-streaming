# IoT Core to Kinesis Firehose to S3 Pipeline

This project sets up an AWS pipeline that ingests data from IoT Core, processes it through Kinesis Firehose, and stores it in S3 as Parquet files, with a Glue table for querying.

## Architecture

- IoT Core: Ingests data from IoT devices
- Kinesis Firehose: Buffers and transforms data
- S3: Stores processed data
- Glue: Provides a queryable table structure

## Features

- Dynamic partitioning based on thing ID and timestamp
- Data conversion from JSON to Parquet
- Error handling with separate error output prefix
- Glue table for easy querying of stored data

## Deployment

1. Clone this repository
2. Ensure you have the AWS SAM CLI installed
3. Update the `samconfig.toml` file with your desired configuration
4. Deploy using SAM:

```bash
sam deploy
```

## Configuration

The `samconfig.toml` file contains the sample configuration for the SAM deployment. You can modify this file to change these parameter values or deployment options.

## License

[MIT License](LICENSE)
