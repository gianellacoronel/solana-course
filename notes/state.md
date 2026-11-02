# State

- Unlike other chains where smart contracts often hold their own state internally, Solana programs are stateless.
- To persist data, programs must utilize external **Accounts**.

- The hierarchy consists of three distinct layers:
  1. State: This is the actual data your application needs to modify or persist over time.
  2. Storage: State cannot float freely; it must be stored inside a container known as an Account.
  3. Ownership: To prevent unauthorized changes, an Account must be owned by the specific Program that intends to modify the data within it.

- States are stored in accounts
- Accounts are owned by the program
- When creating accounts
  - Specify space needed to store the states
  - Pay rent (amount depends on space)
  - Account to be created must sign to prove existence
