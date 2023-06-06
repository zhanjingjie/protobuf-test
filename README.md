## Steps to reproduce the error

`buf generate`

`cd protos/gen/go/company/testservice/testservice/v1`

`go mod init github.com/protobuf-test/grpc/testservice/testservicev1`

`go mod tidy`

Error:
```
go: finding module for package github.com/zhanjingjie/protobuf-test/protos/gen/go/company/protobuf
github.com/protobuf-test/grpc/testservice/testservicev1 imports
        github.com/zhanjingjie/protobuf-test/protos/gen/go/company/protobuf: cannot find module providing package github.com/zhanjingjie/protobuf-test/protos/gen/go/company/protobuf: module github.com/zhanjingjie/protobuf-test/protos/gen/go/company/protobuf: git ls-remote -q origin in /Users/jzhan/go/pkg/mod/cache/vcs/3dca4b2c3933d4b9b98730bb17639229ca9e37986978adc08bc3c6a1699c1c1c: exit status 128:
        remote: Repository not found.
        fatal: repository 'https://github.com/zhanjingjie/protobuf-test/' not found
```