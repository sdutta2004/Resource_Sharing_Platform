![LANDING](https://github.com/user-attachments/assets/c7ca29e4-797e-48bc-b961-9c2935fbad04)
![WALLET](https://github.com/user-attachments/assets/3793f6b5-3478-4da4-ae00-63a3e1f04741)

# 🚀 Resource Sharing Smart Contract (Soroban - Rust)

A decentralized **Resource Sharing Smart Contract** built using **Rust** and **Soroban SDK** on the **Stellar blockchain**.

This contract enables users to:

* 📦 List resources
* 🤝 Borrow & return items
* ⭐ Rate transactions
* 📊 Track availability

---

## 🌐 Live Contract (Testnet)

🔗 https://stellar.expert/explorer/testnet/contract/CBNO3MAH4HDJWEQOSIA2UBHUCUX3XU5XEIEFZD7EWBXDQHGAPLASN5D3

---

## 🧠 Overview

This project implements a **decentralized sharing economy system** where users can list items and allow others to borrow them securely.

Each resource includes:

* Owner details
* Description & category
* Pricing & deposit
* Borrow status
* Ratings & usage stats

---

## ⚙️ Features

### 📌 1. List Resource

* Owners can list a resource with:

  * Name
  * Description
  * Category
  * Daily rate
  * Deposit requirement

---

### 🤝 2. Borrow Resource

* Users can borrow available resources
* Validates:

  * Availability
  * Date range
* Updates borrow count & status

---

### 🔄 3. Return Resource

* Borrower returns the resource
* Adds condition notes
* Updates availability count

---

### ⭐ 4. Rate Transaction

* Users can rate from **1 to 5**
* Maintains:

  * Total rating
  * Rating count

---

### 📊 5. Query Functions

* Get single resource
* List all resources
* Check available resource count

---

## 🏗️ Tech Stack

* 🦀 Rust (`#![no_std]`)
* ⭐ Soroban SDK
* 🌐 Stellar Blockchain

---

## 📁 Smart Contract Structure

### 🔹 Main Struct

```rust
SharedResource
```

Contains:

* Owner & borrower
* Resource details
* Status (`available`, `borrowed`, `returned`)
* Ratings & usage stats

---

### 🔹 Storage Keys

```rust
ResourceDataKey
```

* `IdList` → All resource IDs
* `Item(Symbol)` → Individual resource
* `AvailableCount` → Total available items

---

### 🔹 Errors

```rust
ResourceError
```

Handles:

* Invalid input
* Unauthorized access
* Resource not found
* Invalid rating
* Date issues

---

## 🔐 Security Features

* ✅ Authentication using `require_auth()`
* ✅ Prevents invalid access
* ✅ Safe state transitions
* ✅ Input validation

---

## 📌 Core Functions

| Function              | Description            |
| --------------------- | ---------------------- |
| `list_resource`       | Add new resource       |
| `borrow_resource`     | Borrow an item         |
| `return_resource`     | Return borrowed item   |
| `rate_transaction`    | Rate resource          |
| `get_resource`        | Fetch resource details |
| `list_resources`      | Get all resource IDs   |
| `get_available_count` | Available items count  |

---

## 🚀 How It Works

1. User lists a resource
2. Resource becomes **available**
3. Another user borrows it
4. Status → `borrowed`
5. After return → `returned`
6. Users rate the experience

---

## 📈 Future Improvements

* 💳 Payment integration
* 📅 Advanced booking system
* 🧾 Rental history tracking
* 🌍 Frontend UI (React / Next.js)
* 🔔 Notification system

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a new branch
3. Commit changes
4. Open a Pull Request

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 💡 Author

Built with ❤️ using Rust & Web3 vision.

---

⭐ If you like this project, don't forget to **star the repo!**

