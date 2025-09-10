# 🚀 Sui NFT Workshop – My First On-Chain NFT

Welcome to my **mini workshop project** on Sui ✨  
This repo contains a simple Move contract that mints NFTs with a `name`, `description`, and `image_url`.

And yes… I actually deployed it on **Sui Testnet** 😏  

---

## 📦 Contract Info

- **Module name**: `my_nft`
- **Package ID**: [`0x448c3a8d66a1d909b99d6252e32a24f3896e15646c2d5cc31bf3f5654185166f`](https://explorer.sui.io/package/0x448c3a8d66a1d909b99d6252e32a24f3896e15646c2d5cc31bf3f5654185166f?network=testnet)
- **Publisher address**: [`0xb1fb2ebf34ab432fe3656b10d871d5d5601b42fa9bde2ab713db0842194e9f6f`](https://explorer.sui.io/address/0xb1fb2ebf34ab432fe3656b10d871d5d5601b42fa9bde2ab713db0842194e9f6f?network=testnet)

---

## ✅ Proof of Deployment

| Action        | Explorer Link                                                                                                                                                     |
|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 📦 Publish tx | [HhJtTy9CkYhL7zKY9PnzX3Y1aQavQN7TG4jyTRPzfABW](https://explorer.sui.io/transaction/HhJtTy9CkYhL7zKY9PnzX3Y1aQavQN7TG4jyTRPzfABW?network=testnet) |

*(Mint tx + Object ID can be added here once you mint your first NFT!)*  

---

## 🔧 How I Did It

```bash
# build locally
sui move build

# publish to testnet
sui client publish . --gas-budget 100000000

# mint NFT
sui client call \
  --package 0x448c3a8d66a1d909b99d6252e32a24f3896e15646c2d5cc31bf3f5654185166f \
  --module my_nft \
  --function mint \
  --args "My Cool NFT" "This is a description for my NFT" "https://example.com/image.png" \
  --gas-budget 100000000

🖼️ Screenshots

Proof or it didn’t happen 😏

(Add your screenshots here — publish tx, mint tx, object explorer view)

🌈 What’s Next?

Add a recipient param → so I can mint directly to a friend’s address

Build a small React frontend to connect wallet + click “Mint”

Maybe drop a mini NFT collection? 🤔

✨ Author

Made with 🧑‍💻 + ☕ by Saumya
GitHub