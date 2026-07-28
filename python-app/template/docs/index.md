# ${{values.app_name}}

Documentation for the **${{values.app_name}}** service.

## API endpoints

This application exposes two endpoints:

| Endpoint | Description |
|----------|-------------|
| `GET /api/v1/details` | Returns the current time, hostname, and a status message |
| `GET /api/v1/healthz` | Health check; returns `{"status": "up"}` when the app is running |

### Example URLs

- `https://${{values.app_name}}-${{values.app_env}}.test.com/api/v1/details`
- `https://${{values.app_name}}-${{values.app_env}}.test.com/api/v1/healthz`

## How to access the app

Open the health endpoint in your browser or with `curl`:

```bash
curl https://${{values.app_name}}-${{values.app_env}}.test.com/api/v1/healthz
```

For full details (time, hostname, message):

```bash
curl https://${{values.app_name}}-${{values.app_env}}.test.com/api/v1/details
```
