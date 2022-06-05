# Web-server with Prometheus instrumentation project example

Run the project

```bash
cargo run
```
or if you want to see debus logs

```bash
RUST_LOG=debug cargo run
```

check the metrics endpoint

```bash
curl http://127.0.0.1:3031/metrics
```


check the some endpoint

```bash
curl http://127.0.0.1:3031/some
```

connect to the web-socket endpoint using a tool like websocat
```
websocat -t ws://127.0.0.1:3031/ws/my-client-id
```
