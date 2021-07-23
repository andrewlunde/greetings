```
git add .
git commit -m "greetings: changes for v0.1.0"
git tag v0.1.0
git push origin v0.1.0
GOPROXY=proxy.golang.org go list -m github.com/andrewlunde/greetings@v0.1.0

go get github.com/andrewlunde/greetings@v0.1.0

// in go.mod of application using this module
require greetings v0.0.0
replace greetings v0.0.0 => github.com/andrewlunde/thetaoffchaingo_greetings v0.1.0

```

