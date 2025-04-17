# sentrygin-without-tracing
[github.com/getsentry/sentry-go/blob/master/gin/sentrygin.go](https://github.com/getsentry/sentry-go/blob/v0.32.0/gin/sentrygin.go) but tracing code removed.

## Why
When you have tracing part implemented with OpenTelemetry (e.g [otelgin](https://github.com/open-telemetry/opentelemetry-go-contrib/blob/main/instrumentation/github.com/gin-gonic/gin/otelgin/gin.go)), there is no need for sentrygin to start additional transactions.
