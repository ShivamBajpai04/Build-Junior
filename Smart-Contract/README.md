# Token Airdrop Smart Contract

This Go-based smart contract implements a token airdrop system on the Kalp blockchain.

## Prerequisites

- Go version `>=1.19` but `<1.20`
- Kalp Studio account

## Setup

1. Navigate to the Smart-Contract directory:
   ```bash
   cd Smart-Contract
   ```

2. Install dependencies:
   ```bash
   go mod tidy
   ```

## Smart Contract Functions

- `Initialize(name string, symbol string, decimals string) (bool, error)`: 
  Set up token metadata (name, symbol, decimals)
- `Claim(sdk kalpsdk.TransactionContextInterface, amount int, address string) error`: 
  Mint new tokens and assign them to an address
- `BalanceOf(sdk kalpsdk.TransactionContextInterface, account string) (int, error)`: 
  Check the token balance of an account
- `TotalSupply(sdk kalpsdk.TransactionContextInterface) (int, error)`: 
  Get the total number of tokens in circulation
- `TransferFrom(sdk kalpsdk.TransactionContextInterface, from string, to string, value int) error`: 
  Transfer tokens between accounts

## Deployment

1. Sign up and log in to the Kalp Studio Platform
2. Create a new smart contract project
3. Upload the `krc.go` file
4. Deploy the smart contract using Kalp Studio
5. Generate API endpoints for each function
6. Generate an API key for authentication

## Testing

To run tests (if available):

## Contributing

[Add contribution guidelines]

## License

[Add your license information here]