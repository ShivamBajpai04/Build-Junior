## Running the Application

1. Start the development server:
   ```bash
   npm run dev
   ```

2. Open `http://localhost:3000` in your web browser

## Features

- Claim tokens: Users can claim a predefined amount of tokens
- Check token balances: Users can view their current token balance
- View total supply: Display the total number of tokens in circulation
- Transfer tokens: Users can send tokens to other addresses

## Project Structure

- `src/hooks/useKalpAPI.tsx`: Custom hook for Kalp API interactions
- `src/app/page.tsx`: Main application component
- `.env.local`: Environment variables (API key)
- `public/`: Static assets

## API Interactions

The `useKalpAPI` hook in `src/hooks/useKalpAPI.tsx` handles all interactions with the Kalp blockchain. It provides the following functions:

- `claim(address: string)`: Mint new tokens for the given address
- `balanceOf(account: string)`: Get the token balance of an account
- `totalSupply()`: Get the total supply of tokens
- `transferFrom(from: string, to: string, value: number)`: Transfer tokens between accounts

## Contributing

1. Fork the repository
2. Create a new branch for your feature
3. Make your changes
4. Run tests (if available) and ensure they pass
5. Submit a pull request with a comprehensive description of changes

## License

[Add your license information here]

## Troubleshooting

- If you encounter API errors, check your API key and endpoint configurations
- For React-related issues, ensure all dependencies are correctly installed
- Check the browser console for any error messages

For more information on Next.js, check out [the Next.js documentation](https://nextjs.org/docs).