goad
====

`goad` is an alarming shell script used to build golang projects.

It's a template -- copy it and set your project path in the env vars at the top.

You're expected to set a symlink from `./.gopath/src/github.com/youruser/yourproject/` back up to `../../../../../` (e.g. the repo root).
This causes your package import path to be the same when you're using self-contained project-relative build paths, and also when someone is looking at you through the rose-tinted glasses of `go get`.

Add git submodules in a similar pattern under `./.gopath/src/` to get a self contained, deterministic project build environment with no additional fuss.


