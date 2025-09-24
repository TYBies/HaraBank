# HaraBank

A modern banking platform for seamless account management, transaction tracking, and money transfers—including upcoming international remittance support.

## Features

- **User Authentication:** Secure sign up and login
- **Bank Account Linking:** Connect US bank accounts via Plaid
- **Funds Transfer:** Move money between US accounts using Dwolla ACH
- **Transaction History & Categorization:** Track and analyze your financial activity
- **Dashboard:** View balances, recent transactions, and analytics
- **International Remittance (Coming Soon):**  
  Send money to African banks and mobile wallets using cheapest and fastest channels (Wise, Flutterwave, Paystack, etc.)

## Supported Providers

- **Plaid:** For linking US bank accounts
- **Dwolla:** For initiating US domestic ACH transfers
- **Wise, Flutterwave, Paystack (Planned):** For fast, low-cost remittance to Africa

## Setup Instructions

1. **Clone the repository**
2. **Install dependencies**  
   ```bash
   npm install
   ```
3. **Set environment variables:**  
   See `.env.example` for required keys (Plaid, Dwolla, etc.)
4. **Run the app**  
   ```bash
   npm run dev
   ```

## Linking Your Bank

1. Authenticate and sign in
2. Use the “Connect bank” button (Plaid Link) to add your US account
3. Complete verification—your account is now ready for transfers

## Transferring Funds

- **US Transfers:**  
   Select source and destination accounts, enter amount, and confirm. Transfers processed via Dwolla ACH.

- **International Remittance (Coming Soon):**  
   Choose recipient country, payout method (bank/mobile money), and complete KYC. Funds sent via Wise/Flutterwave/Paystack.

## Environment Configuration

- Set `DWOLLA_ENV=sandbox` for testing, `DWOLLA_ENV=production` for live transfers
- API keys for Plaid, Dwolla, and (when available) Wise/Flutterwave/Paystack must be set in your environment

## Compliance & KYC

- US transfers require Dwolla customer verification
- International remittance will require sender and recipient KYC per provider/regulation

## Contributing

Pull requests, issues, and suggestions are welcome!  
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

**Note:**  
International remittance to Africa is under development. If you want to help, check out the [issues](https://github.com/TYBies/HaraBank/issues) or contact the maintainer.