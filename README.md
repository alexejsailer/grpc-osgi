# grpc-osgi
Self-contained io.grpc OSGi bundle

http://creativecommons.org/licenses/by-nc-nd/3.0/

[![Foo](https://www.dualexec.com/wiki/lib/tpl/markgard-gtopia-wiki-c621a539da50/images/88x31.png)](http://creativecommons.org/licenses/by-nc-nd/3.0/de/)

[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" width="150">](https://www.buymeacoffee.com/alexejsailer)

To build this project run:

```shell
mvn clean install
``` 

Copy your built bundle from the target folder and copy all below mentioned dependencies from maven or use the following command if you are using karaf:

```shell
bundle:install mvn:com.google.protobuf/protobuf-java/3.12.4
bundle:install mvn:com.google.protobuf.nano/protobuf-javanano/3.1.0
bundle:install mvn:io.grpc/grpc-osgi/1.31.1
```

You will now be able to start a complete grpc server in a separate custom bundle. Therefore you should define your proto file first and generate java code form it. I will provide an example on demand.
