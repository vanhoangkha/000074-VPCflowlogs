# Monitoring network infrastructure

> Network monitoring with VPC Flow Logs.

A hands-on workshop from the [AWS First Cloud Journey](https://github.com/vanhoangkha/aws-first-cloud-journey) series, available in English and Vietnamese.

**Read the workshop online:** https://vanhoangkha.github.io/000074-VPCflowlogs/

## Overview

VPC Flow Logs is a feature that allows you to monitor information about IP traffic to and from network interfaces in your VPC. Stream log data can be published to Amazon CloudWatch Logs or Amazon S3. After creating a stream log, you can retrieve and view its data at the selected destination.

In this lab, Stream data will be published to Amazon CloudWatch Logs.

## Workshop contents

1. Introduction
2. Preparation
3. Create VPC Flow Logs
4. Enable VPC Flow Logs
5. Network Infrastructure Monitoring
6. Clean up resources

## Prerequisites

- An AWS account with permissions to create the resources used in the labs
- Basic familiarity with the AWS Management Console
- [Hugo](https://gohugo.io/installation/) (extended edition) if you want to run the site locally

## Run locally

```bash
git clone https://github.com/vanhoangkha/000074-VPCflowlogs.git
cd 000074-VPCflowlogs
hugo server
```

Then open http://localhost:1313 in your browser.

## Repository structure

| Path | Purpose |
| --- | --- |
| `content/` | Workshop pages (`*.md` English, `*.vi.md` Vietnamese) |
| `static/` | Images and other static assets |
| `layouts/` | Hugo layout overrides |
| `themes/` | Hugo theme |
| `config.toml` | Site configuration |

## Cost and cleanup

The labs create AWS resources that may incur charges. Complete the **Clean up** chapter when you finish to remove them.

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

To report a security issue, see [SECURITY.md](SECURITY.md).

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
