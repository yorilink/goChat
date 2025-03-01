妈的傻逼npm
第一个坑正常安装npm，但是会把可执行文件pbjs.cmd 安装到cache里。 把cache里的文件迁移过去
第二个坑在生成proto.js文件时  直接 pbjs --es6 protogen/chat_pb.js protos/chat.proto 就可以了。

{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "type": "chrome",
            "request": "launch",
            "name": "Debug Frontend",
            "url": "http://localhost:8080",
            "webRoot": "${workspaceFolder}"
        },
        {
            "type": "go",
            "request": "launch",
            "name": "Debug Go Server",
            "mode": "debug",
            "program": "${workspaceFolder}",
            "args": [],
            "env": {},
            "showLog": true,
            "trace": "verbose"
        },
        {
            "name": "Debug Frontend and Go Server",
            "type": "compound",
            "configurations": ["Debug Frontend", "Debug Go Server"]
        }
    ]
}