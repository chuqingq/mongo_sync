# mongo_sync

Sync mongo replica-set by go, and can resume from last breakpoint(timestamp saved `ts` in configuration file).

## configuration

`sync.conf`:

```json
{
    "src": {
        "addrs": "192.168.25.89:20001",
        "username": "user",
        "password": "pass"
    },
    "dst": {
        "addrs": "192.168.25.84:20001",
        "username": "user",
        "password": "pass"
    },
    "bufsize": 10000,
    "ns": [
        "chuqq.*",
        "chuqqtest.*"
    ],
    "ts": 0
}
```

