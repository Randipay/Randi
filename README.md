# Randi

**Stellar-Powered Payment Requests for South African Businesses**

Randi is a payment-request platform built on the Stellar network that enables businesses and freelancers to create simple payment requests, share them with customers, and receive USDC payments on Stellar Testnet.

The MVP allows merchants to create a payment request denominated in South African Rand (ZAR), provide a payment page to the customer, detect the corresponding Stellar payment, and automatically verify the transaction.

> **Network:** Stellar Testnet  
> **Status:** MVP  
> **Settlement Asset:** USDC  
> **Primary Market:** South Africa

---

## Overview

Businesses and freelancers need simple ways to request and confirm digital payments.

Crypto payments can introduce additional friction through long wallet addresses, asset selection, payment references, and manual transaction verification.

Randi simplifies this process by providing a payment-request layer where the merchant specifies the amount in ZAR while the actual settlement occurs using USDC on Stellar Testnet.

### Core Flow

**Create Payment Request → Share Payment Page → Customer Pays USDC → Stellar Payment Detected → Payment Verified → Marked Paid**

---

## Problem

Businesses and freelancers accepting digital-asset payments often need to:

- Create payment requests manually
- Share long wallet addresses
- Provide payment instructions to customers
- Manually check blockchain transactions
- Confirm whether the correct amount was received
- Track completed and pending payments

This creates unnecessary friction for both merchants and customers.

---

## Solution

Randi provides a simple payment-request workflow for businesses and freelancers.

A merchant can:

1. Create a payment request.
2. Specify the amount in ZAR.
3. Provide their Stellar wallet address.
4. Generate a unique payment request.
5. Share the payment page with a customer.
6. Receive USDC on Stellar Testnet.
7. Automatically verify the payment.
8. View the payment status and transaction hash.

---

## Features

### Payment Request Creation

Merchants can create payment requests containing:

- ZAR-denominated amount
- Supported payment asset
- Stellar recipient address
- Unique payment ID
- Payment reference
- Expiry time
- Payment status

### Payment Page

Customers can view:

- Merchant information
- Requested amount
- Payment asset
- Payment instructions
- Recipient information
- Payment status
- Transaction confirmation

### Stellar Payment Detection

Randi monitors Stellar Testnet for incoming payments associated with active payment requests.

### Payment Verification

Payments are checked against:

- Recipient address
- Asset
- Expected amount
- Payment reference
- Payment request status

A valid payment changes the request from:

```text
Pending
   ↓
Paid
