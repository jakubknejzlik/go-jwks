# JSON Web Key Client

Client code which fetches from a public JWKs endpoint. This client maintains an
in-memory cache of keys by id.

## Installation
```
go get github.com/jakubknejzlik/go-jwks
```

## Usage

```go
client := jwks.NewClient("https://yourdomain.auth0.com/.well-known/jwks.json")

// Inside handler func...
key, err := c.GetKey("akdflasjfpoasdkfja")
// Use key to validate JWT...
```
