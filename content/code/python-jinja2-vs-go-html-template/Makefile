# cannot use relative path in GOROOT, otherwise 6g not found. For example,
#   export GOROOT=../go  (=> 6g not found)
# it is also not allowed to use relative path in GOPATH
export GOROOT=$(realpath ../../../../../go)
export GOPATH=$(realpath .)
export PATH := $(GOROOT)/bin:$(PATH)

# path of Google App Engine Python SDK
GAE_PY_SDK=../../../../../google_appengine

all: example5

example1:
	@# http://stackoverflow.com/questions/9967105/suppress-echo-of-command-invocation-in-makefile
	@python jinja2-example-1.py
	@go run html-template-example-1.go

example2:
	@python jinja2-example-2.py
	@go run html-template-example-2.go

example3:
	@python jinja2-example-3.py
	@go run html-template-example-3.go

example4:
	@python jinja2-example-4.py
	@go run html-template-example-4.go

example5:
	@python jinja2-example-5.py
	@python jinja2-example-5_1.py
	@go run html-template-example-5.go

help:
	go help
