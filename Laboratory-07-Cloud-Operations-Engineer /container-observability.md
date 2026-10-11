# Container Observability Report

## Application Logging

**404 Error Log:**

Paste the exact line from your `docker logs client-website` output that contains `GET /hidden-admin-page` and the status code `404`.

**Why Application Logs Are Important**

Application logs help identify errors, failed requests, and unusual application behavior. They allow engineers to trace problems, understand what happened, and determine the appropriate solution.

## Log Monitoring Command

```bash
docker logs client-website
```

## Real-Time Container Metrics

- **Container Name:** `client-website`
- **Memory Usage:** 2.75 MiB
- **CPU Percentage:** 0.00%
