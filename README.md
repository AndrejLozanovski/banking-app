## BankingApp

BankingApp is a financial SaaS platform built with NextJS that displays transactions in real-time, connects to multiple bank accounts, manages their finances and allows users to transfer money to other platform users.

## Tech Stack
<p align="center">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img src="https://img.shields.io/badge/Appwrite-F02E65?style=for-the-badge&logo=appwrite&logoColor=white" />
  <img src="https://img.shields.io/badge/Plaid-0085CA?style=for-the-badge&logo=plaid&logoColor=white" />
  <img src="https://img.shields.io/badge/Dwolla-FF5C00?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Zod-2F80ED?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/React Hook Form-EC5990?style=for-the-badge&logo=reacthookform&logoColor=white" />
  <img src="https://img.shields.io/badge/ShadCN-FFFFFF?style=for-the-badge&logoColor=black" />
</p>

## Features
 - **HomePage**: Here is displayed the general overview of users account with total balance from all connected banks, the transactions, bank cards
 - **My Banks**: List of all connected banks with their balances and account details
 - **Real-time Updates**: Reflects changes across all relevant pages upon connecting new bank accounts
 - **Authentication**: Secure SSR authentication with validations and authorization
 - **Connect Banks**: Integrates with Plaid for multiple bank account linking
 - **Fund Transfer**: Allows users to transfer funds using Dwolla to other accounts with required fields and recipient bank ID
 - **Responsive**: The application adapts seamlessly to various screen sizes and devices

## Prerequisites
To run the project, you'll need:
  - Git
  - Node.js
  - npm

## Installation
**1.Clone the repository:**
```bash
  git clone https://github.com/AndrejLozanovski/banking-app.git
  cd banking-app
```     
**2.Open the terminal and Install the dependencies** <br>
```bash
  npm install
```
     
**Setup environment variables:** <br>
     Create a ```.env``` file and add: <br><br>
     
      ```sh
      
      #NEXT
      NEXT_PUBLIC_SITE_URL=

      #APPWRITE
      NEXT_PUBLIC_APPWRITE_ENDPOINT=
      NEXT_PUBLIC_APPWRITE_PROJECT=
      APPWRITE_DATABASE_ID=
      APPWRITE_USER_COLLECTION_ID=
      APPWRITE_BANK_COLLECTION_ID=
      APPWRITE_TRANSACTION_COLLECTION_ID=
      APPWRITE_SECRET=
      
      #PLAID
      PLAID_CLIENT_ID=
      PLAID_SECRET=
      PLAID_ENV=
      PLAID_PRODUCTS=
      PLAID_COUNTRY_CODES=
      
      #DWOLLA
      DWOLLA_KEY=
      DWOLLA_SECRET=
      DWOLLA_BASE_URL=
      DWOLLA_ENV=

  Enter the values with your actual respective account credentials, you can obtain them by signing up on Appwrite, Plaid and Dwolla
  
**Run the project**
    
    ```sh
    npm run dev
    
    
  And open https://localhost:3000 in your browser
