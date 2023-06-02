# Project setup
## Create a 'properties.env' file in './configs' directory with the following content
DB_USER=encora   
DB_PASS=encora   
DB_NAME=go-challenges   
BEARER_TOKEN=Bearer encoraBearerTokenGoChallenges   
DB_IMPL=(orm or vanilla)

---

# REST setup
## Running the REST server
`go run cmd/rest/*.go`

---

# gRPC setup
## Generating .proto files
`make clean`   
`make build`

or

`bash ./scripts/grpc/grpc-setup.sh`

## Running the gRPC server
`go run cmd/grpc-server/*.go`

## Running the gRPC client
`go run cmd/grpc-client/*.go`
