\# Laboratory Activity 5 Reflection: The Cloud Data Engineer



\## Key Learnings

1\. \*\*Object Storage vs. Block Storage\*\*: Object storage (like S3 and MinIO) manages data as discrete objects paired with rich metadata, making it ideal for unstructured data such as photos, media, and backups, whereas block storage is tailored for low-latency database engines.

2\. \*\*S3 API Compatibility\*\*: Running MinIO locally provides full compatibility with the AWS S3 API, allowing seamless development and testing of cloud data pipelines before deploying to public cloud providers like AWS.

3\. \*\*Service Management \& Binding\*\*: Configuring service listening interfaces (`0.0.0.0` vs `127.0.0.1`) is critical when exposing cloud applications through proxies or container port forwarding.



\## Challenges \& Solutions

\- \*\*Challenge\*\*: Encountered registry network restrictions and binary download errors when deploying MinIO.

\- \*\*Solution\*\*: Compiled and deployed the native MinIO binary, configuring environment variables and explicit console bindings (`0.0.0.0:9001`) to allow external network access via KillerCoda port accessor.

