# StepCash - Real Money Walking App

Earn real cash for every step you take. Walk, track, earn, and withdraw to PayPal, bank, or gift cards.

## Features
- 🚶 Real-time step tracking using device sensors
- 💰 Automatic earnings calculation ($0.50 per 10,000 steps)
- 🏦 Real money withdrawals (PayPal, Bank Transfer, Gift Cards)
- 🎯 Daily goals and streak bonuses
- 👥 Referral system ($5 per friend)
- 📊 Earnings analytics and charts
- 📱 PWA - Install as native app
- 🔒 Secure authentication and transactions

## Tech Stack
- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Backend**: Firebase (Auth, Firestore, Functions)
- **Payments**: Stripe, PayPal, Gift Cards
- **Hosting**: Firebase Hosting
- **Email**: SendGrid

## Setup Instructions

### 1. Firebase Setup
1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create new project: `StepCash-Production`
3. Enable services:
   - Authentication (Email/Password, Google)
   - Firestore Database
   - Cloud Functions
   - Hosting

### 2. Stripe Setup
1. Sign up at [Stripe](https://stripe.com)
2. Get API keys (Test and Live)
3. Enable Stripe Connect
4. Add your bank account

### 3. PayPal Setup (Optional)
1. Create PayPal Business account
2. Enable Payouts API
3. Get Client ID and Secret

### 4. Email Setup (SendGrid)
1. Sign up at [SendGrid](https://sendgrid.com)
2. Verify sender email
3. Get API key

### 5. Environment Configuration
1. Copy `.env.example` to `.env`
2. Fill in all your API keys and credentials
3. For Cloud Functions, set environment variables:
```bash
firebase functions:config:set stripe.secret="sk_live_xxx"
firebase functions:config:set sendgrid.api_key="SG.xxx"
