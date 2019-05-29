# gogoslim

A customized gogoprotobuf to generate fast & slim code (without `XXX_shit` fields and `GetShit()` methods)

## Usage

```
go get -u github.com/lqs/gogoslim/protoc-gen-gogoslim

protoc -I. --gogoslim_out=\
Mgoogle/protobuf/any.proto=github.com/lqs/gogoslim/types,\
Mgoogle/protobuf/duration.proto=github.com/lqs/gogoslim/types,\
Mgoogle/protobuf/empty.proto=github.com/lqs/gogoslim/types,\
Mgoogle/protobuf/struct.proto=github.com/lqs/gogoslim/types,\
Mgoogle/protobuf/timestamp.proto=github.com/lqs/gogoslim/types,\
Mgoogle/protobuf/wrappers.proto=github.com/gogo/protobuf/types:. \
myproto.proto
```
