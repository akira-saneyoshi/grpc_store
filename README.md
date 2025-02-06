# grpc_store

```zsh
cd /tmp/protoc
sudo apt install unzip curl
PROTOC_VERSION=$(curl -s "https://api.github.com/repos/protocolbuffers/protobuf/releases/latest" | grep -Po '"tag_name": "v\K[0-9.]+')
wget -qO protoc.zip https://github.com/protocolbuffers/protobuf/releases/latest/download/protoc-$PROTOC_VERSION-linux-x86_64.zip
unzip protoc.zip
mv /tmp/protoc/bin/* /usr/local/bin/
mv /tmp/protoc/include/* /usr/local/include
rm -rf protoc protoc.zip
sudo apt install  protobuf-dev
```
