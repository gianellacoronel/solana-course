## Accounts

- All data on Solana are stored in accounts.
- An account could be:
  - `executable = true` => Program account.
  - `executable = false` => Data account.

### Examples

1. Wallet as an account

```
Account {
  lamports: 1,000,000,000
  data: []
  owner: System program
  executable: false
}
```

2. Deployed counter program

```
Account {
  lamports: 100,000 (depends on data size)
  data: [0, 1, 255, 123, ...]
  owner: BPF loader program
  executable: true
}
```
