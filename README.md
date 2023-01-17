# lynx-iberian-example

This project has the goal of making the bot as easy to configure as possible.

## How to run Lynx-Iberian

Open a terminal in the project folder and run
```bash
docker compose up
```

You can run it in the background with the following command

**Be careful!** Some plugins may require some initial configuration using the terminal.
Don't run it in the background after installing a plugin!

```bash
docker compose up -d
```


## Common problems

P: Node red is not starting! Error: EACCES: permission denied, copyfile

S: Add the correct permissions to node-red folder
```bash
sudo chown -R 1000:1000 node-red-data
```