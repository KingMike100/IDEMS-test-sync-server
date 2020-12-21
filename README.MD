# IDEMS test Sync Server

## Synopsis

A small node server which uses [NeDB](https://github.com/louischatriot/nedb) to write data to the disk. The server can be used with a client for example [SyncClient](https://github.com/nponiros/sync_client) to save change sets which can later be synchronized with other devices. The server was made to work with the [ISyncProtocol](https://github.com/dfahlander/Dexie.js/wiki/Dexie.Syncable.ISyncProtocol) and [Dexie.Syncable](https://www.npmjs.com/package/dexie-syncable). It supports the poll pattern using AJAX and the react pattern using [nodejs-websocket](https://www.npmjs.com/package/nodejs-websocket).

## Usage

You can start the server with:

```bash
sync-server start --path INIT/DIRECTORY/PATH
```

The `--path` flag must be given the path to the directory in which `server` was stored.