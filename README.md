# pusher 
Simple linux tool for automation `git push` process.
Under the hood it makes three things:

- adds a change in the working directory to the staging area;
- commit changes;
- push changes in the current remote branch.

## Linux installation

1. Clone the current repository: `https://github.com/GolovPavel/pusher.git`;
2. Install `gdebi` package, if you do not have it: `sudo apt-get install gdebi`;
3. Go to the pusher directory: `cd pusher`;
4. Install pusher package: `sudo gdebi "pusher.deb"`.

## Macos installation

1. Clone the current repository: `https://github.com/GolovPavel/pusher.git`;
2. Make `pusher` script executable: `sudo chmod +x pusher/bin/pusher`;
3. Copy script to the one of the `$PATH` directories. For example: `cp pusher/bin/pusher /usr/local/bin`.
4. Restart shell.

## Usage

Push to the remote repository all local changes with some message:

```
pusher "Some message"
```

Push to the remote repository all local changes with default message:

```
pusher
```

The default message is `Empty commit message`.

When you type `pusher` command, you must be in the local repository directory.
