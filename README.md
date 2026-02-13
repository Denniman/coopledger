# coopLedger

**coopLedger** is a secure, cloud-based web application designed to modernize the financial operations of cooperative societies. It replaces manual record-keeping (WhatsApp, physical cards) with an automated, transparent, and efficient digital system.

## 🚀 Project Overview

The primary goal of coopLedger is to streamline financial tracking, loan management, and reporting for cooperative members and administrators. It ensures real-time accuracy, automates complex calculations (interest, fines, eligibility), and provides clear audit trails.

## ✨ Key Features

- **Role-Based Access Control (RBAC)**: Distinct dashboards and permissions for Regular Members, Chairman, and Financial Secretary.
- **Transaction Management**: Record, verify, and approve contributions and withdrawals with an approval workflow.
- **Automated Financials**: Real-time calculation of Member Gross/Net Worth, Loan Eligibility, and Cooperative Total Worth.
- **Loan Management System**:
  - Automated eligibility checks based on net worth.
  - Instant loan repayment schedule generation (Principal + 10% Interest).
  - Automatic tracking of repayments and application of late fines.
- **Comprehensive Reporting**: Generate PDF/Excel reports for Annual Financials, Individual Statements, and Defaulters.
- **Security**: Invite-only registration, secure authentication, and detailed audit logs.

## 🛠️ Tech Stack

This project is built as a **Monorepo** using **TurboRepo**.

### Frontend (`apps/web`)

- **Framework**: [Next.js 15](https://nextjs.org/) (App Router)
- **Language**: TypeScript
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **UI Components**: [ShadCN UI](https://ui.shadcn.com/)
- **Package Manager**: pnpm

### Backend (`apps/api`)

- **Runtime**: Node.js
- **Framework**: Express.js
- **Language**: TypeScript
- **Architecture**: Modular Monolith

## 📂 Project Structure

```
coopLedger/
├── apps/
│   ├── web/    # Next.js Frontend Application
│   └── api/    # Express Backend Application
├── packages/   # Shared packages (if any)
├── turbo.json  # TurboRepo configuration
└── package.json
```

## ⚡ Getting Started

### Prerequisites

- Node.js (v18+)
- pnpm (v9+)

### Installation

1.  Clone the repository:

    ```bash
    git clone git@github.com:Denniman/coopledger.git
    cd coopLedger
    ```

2.  Install dependencies:
    ```bash
    pnpm install
    ```

### Development

To start the development server for all apps (Frontend & Backend):

```bash
pnpm dev
```

- **Frontend**: [http://localhost:3000](http://localhost:3000)
- **Backend**: [http://localhost:3001](http://localhost:3001)

### Building

To build all apps for production:

```bash
pnpm build
```

### Linting & Formatting

We use **ESLint**, **Prettier**, and **Husky** to ensure code quality.

```bash
pnpm lint      # Run linting
pnpm format    # Run formatting
```

## 📄 Documentation

- [Product Requirements Document (PRD)](./coopLedger-prd.md)
- [Technical Architecture](./coopLedger-technical-architecture.md)

## 🤝 Contributing

1.  This is a private repository for the cooperative society.
2.  Ensure all code passes linting checks before committing.
3.  Use meaningful commit messages.

## 📝 License

Private & Confidential.
