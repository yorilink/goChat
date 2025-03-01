妈的傻逼npm
第一个坑正常安装npm，但是会把可执行文件pbjs.cmd 安装到cache里。 把cache里的文件迁移过去
第二个坑在生成proto.js文件时  直接 pbjs --es6 protogen/chat_pb.js protos/chat.proto 就可以了。

