
# signal-desktop-docker

Reproducer for signal-desktop error. Run `build` and then `runme signal-desktop`.

```
NODE_ENV production
NODE_CONFIG_DIR /usr/lib/signal-desktop/resources/app.asar/config
NODE_CONFIG {}
ALLOW_CONFIG_MUTATIONS undefined
HOSTNAME undefined
NODE_APP_INSTANCE undefined
SUPPRESS_NO_CONFIG_WARNING undefined
SIGNAL_ENABLE_HTTP undefined
userData: /home/signal/.config/Signal
config/get: Did not find user config file, cache is now empty object
Set Windows Application User Model ID (AUMID) { appUserModelId: 'org.whispersystems.signal-desktop' }
x-attr dependency did not load successfully
config/get: Did not find ephemeral config file, cache is now empty object
making app single instance
key/initialize: Generating new encryption key, since we did not find it on disk
config/set: Saving user config to disk
libGL error: MESA-LOADER: failed to retrieve device information
libGL error: Version 4 or later of flush extension not found
libGL error: failed to load driver: i915
libGL error: failed to open /dev/dri/card0: No such file or directory
libGL error: failed to load driver: i965
j{"level":30,"time":"2021-08-14T20:45:52.493Z","pid":1,"hostname":"1b6c8b7a1205","msg":"app ready"}
{"level":30,"time":"2021-08-14T20:45:52.496Z","pid":1,"hostname":"1b6c8b7a1205","msg":"starting version 5.13.0"}
{"level":30,"time":"2021-08-14T20:45:52.496Z","pid":1,"hostname":"1b6c8b7a1205","msg":"media access status"}
migrateSchemaVersion: Migrating from schema_version 0 to user_version 0
migrateDatabase: Migration without cipher change failed
Database startup error: SqliteError: file is not a database
    at Database.pragma (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:648:31)
    at getUserVersion (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:23949:15)
    at migrateSchemaVersion (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:23969:25)
    at openAndMigrateDatabase (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:24001:5)
    at openAndSetUpSQLCipher (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:24017:16)
    at Object.initialize (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:25563:14)
    at MessagePort.<anonymous> (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:28224:36)
    at MessagePort.[nodejs.internal.kHybridDispatch] (internal/event_target.js:354:41)
    at MessagePort.exports.emitMessage (internal/per_context/messageport.js:18:26)
Unhandled Promise Rejection: Error: SqliteError: file is not a database
    at Database.pragma (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:648:31)
    at getUserVersion (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:23949:15)
    at migrateSchemaVersion (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:23969:25)
    at openAndMigrateDatabase (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:24001:5)
    at openAndSetUpSQLCipher (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:24017:16)
    at Object.initialize (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:25563:14)
    at MessagePort.<anonymous> (/usr/lib/signal-desktop/resources/app.asar.unpacked/ts/sql/mainWorker.bundle.js:28224:36)
    at MessagePort.[nodejs.internal.kHybridDispatch] (internal/event_target.js:354:41)
    at MessagePort.exports.emitMessage (internal/per_context/messageport.js:18:26)
    at Worker.<anonymous> (/usr/lib/signal-desktop/resources/app.asar/ts/sql/main.js:33:29)
    at Worker.emit (events.js:315:20)
    at MessagePort.<anonymous> (internal/worker.js:207:53)
    at MessagePort.[nodejs.internal.kHybridDispatch] (internal/event_target.js:354:41)
    at MessagePort.exports.emitMessage (internal/per_context/messageport.js:18:26)
{"level":50,"time":"2021-08-14T20:45:52.574Z","pid":1,"hostname":"1b6c8b7a1205","msg":"Unhandled Promise Rejection: Error: SqliteError: file is not a database\n    at Database.pragma ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:648:31)\n    at getUserVersion ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:23949:15)\n    at migrateSchemaVersion ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:23969:25)\n    at openAndMigrateDatabase ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:24001:5)\n    at openAndSetUpSQLCipher ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:24017:16)\n    at Object.initialize ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:25563:14)\n    at MessagePort.<anonymous> ([REDACTED].unpacked/ts/sql/mainWorker.bundle.js:28224:36)\n    at MessagePort.[nodejs.internal.kHybridDispatch] (internal/event_target.js:354:41)\n    at MessagePort.exports.emitMessage (internal/per_context/messageport.js:18:26)\n    at Worker.<anonymous> ([REDACTED]/ts/sql/main.js:33:29)\n    at Worker.emit (events.js:315:20)\n    at MessagePort.<anonymous> (internal/worker.js:207:53)\n    at MessagePort.[nodejs.internal.kHybridDispatch] (internal/event_target.js:354:41)\n    at MessagePort.exports.emitMessage (internal/per_context/messageport.js:18:26)"}
```

