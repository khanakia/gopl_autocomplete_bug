## Go Autocomplete bug gopls

vscode autocomplete intellisense does not works when vendor directory exists


## gopls output when starting vscode
```
[Info  - 19:09:05] 2024/04/15 19:09:05 go info for /Volumes/D/luci/Downloads/goworkspace
(view type GoWorkView)
(root dir /Volumes/D/luci/Downloads/goworkspace)
(go version go version go1.22.1 darwin/arm64)
(build flags: [])
(go env: {GOOS:js GOARCH:wasm GOCACHE:/Volumes/D/khanakia/Library/Caches/go-build GOMODCACHE:/Volumes/D/khanakia/go/pkg/mod GOPATH:/Volumes/D/khanakia/go GOPRIVATE:github.com/theuxm GOFLAGS: GO111MODULE:on GoVersion:22 GoVersionOutput:go version go1.22.1 darwin/arm64
 GOWORK: GOPACKAGESDRIVER:})
(env overlay: map[])


[Info  - 19:09:05] 2024/04/15 19:09:05 go/packages.Load #1
	snapshot=0
	directory=file:///Volumes/D/luci/Downloads/goworkspace
	query=[/Volumes/D/luci/Downloads/goworkspace/app/... /Volumes/D/luci/Downloads/goworkspace/ping/... builtin]
	packages=3

[Info  - 19:09:05] 2024/04/15 19:09:05 go/packages.Load #1: updating metadata for 47 packages

```


## Gops output when i start typeing the package name `ping`
```
[Error - 19:09:17] 2024/04/15 19:09:17 no completions found: err: exit status 1: stderr: go: can't match module patterns using the vendor directory
	(Use -mod=mod or -mod=readonly to bypass.)

	position=5:2
```