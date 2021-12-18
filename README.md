# issue_gyp

Experiments to [issue #2484](https://github.com/nodejs/node-gyp/issues/2484) in `node-gyp`.

Install three modules: deasync, w.process.tree.windows, bufferfromfile

| NodeJs version | Windows-2016         | Windows-2019 ( Windows-latest ) | Windows-2022                |
|----------------|----------------------|---------------------------------|-----------------------------|
| 12.x           | pass                 | pass                            | fail ( wrong GitHub setup ) |
| 14.x           | pass                 | pass                            | fail ( wrong GitHub setup ) |
| 16.x           | fail ( demonstrate ) | fail ( demonstrate )            | fail ( wrong GitHub setup ) |

`wrong GitHub setup` means error message ` You need to install the latest version of Visual Studio` but not problem on Windows-2016, Windows-2019.

Install two modules on Windows-2019 ( Windows-latest ):

| NodeJs version | deasync-wprocess.tree | deasync-bufferfromfile | bufferfromfile-wprocess.tree |
|----------------|-----------------------|------------------------|------------------------------|
| 12.x           | pass                  | pass                   | pass                         |
| 14.x           | pass                  | pass                   | pass                         |
| 16.x           | pass                  | pass                   | pass                         |

