# Azure-Function-App-Insight-Config
### The repo contains a balanced cost/efficiency config of Application Insight for Azure Functions that won't destroy your subscription's billing and would allow to monitor your app.

- Keep **"default"** on Information level to recieve developer's logs and big part of metrics.
- **"maxTelemetryItemsPerSecond"** - how many traces is send per second excluding types from "excludedTypes"
- **"enableDependencyTracking"** - disabling tracking of database, http calls, etc from functions tracking may redice additional costs.
- **"enableLiveMetrics"** - disabling live metrics won't reduce cost.
