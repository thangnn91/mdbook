### 1. Contract address

- [Mainnet - 0x0b10A9a0A42aD00e06Ed7E9bbE25f4055F586215](https://arbiscan.io/address/0x0b10A9a0A42aD00e06Ed7E9bbE25f4055F586215)
- [Testnet - 0x342A5D8FdB25704F1817f07445115a3adF22210D](https://sepolia.arbiscan.io/address/0x342A5D8FdB25704F1817f07445115a3adF22210D)
  <details>
    <summary>Abi</summary>

  ```json
  [
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "_collateral",
          "type": "address"
        },
        {
          "internalType": "address",
          "name": "_ctf",
          "type": "address"
        },
        {
          "internalType": "address",
          "name": "_proxyHelper",
          "type": "address"
        }
      ],
      "stateMutability": "nonpayable",
      "type": "constructor"
    },
    {
      "inputs": [],
      "name": "AlreadyRegistered",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "FeeTooHigh",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "InvalidComplement",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "InvalidNonce",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "InvalidSignature",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "InvalidTokenId",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "MakingGtRemaining",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "MismatchedTokenIds",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "NotAdmin",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "NotCrossing",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "NotOperator",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "NotOwner",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "NotTaker",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "OrderExpired",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "OrderFilledOrCancelled",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "Paused",
      "type": "error"
    },
    {
      "inputs": [],
      "name": "TooLittleTokensReceived",
      "type": "error"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "receiver",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "tokenId",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "amount",
          "type": "uint256"
        }
      ],
      "name": "FeeCharged",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "newAdminAddress",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "NewAdmin",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "newApproverAddress",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "NewApprover",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "newOperatorAddress",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "NewOperator",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "bytes32",
          "name": "orderHash",
          "type": "bytes32"
        }
      ],
      "name": "OrderCancelled",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "bytes32",
          "name": "orderHash",
          "type": "bytes32"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "maker",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "taker",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "makerAssetId",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "takerAssetId",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "makerAmountFilled",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "takerAmountFilled",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "fee",
          "type": "uint256"
        }
      ],
      "name": "OrderFilled",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "bytes32",
          "name": "takerOrderHash",
          "type": "bytes32"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "takerOrderMaker",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "makerAssetId",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "takerAssetId",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "makerAmountFilled",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "takerAmountFilled",
          "type": "uint256"
        }
      ],
      "name": "OrdersMatched",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "oldAddress",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "newAddress",
          "type": "address"
        }
      ],
      "name": "ProxyHelperUpdated",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "removedAdmin",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "RemovedAdmin",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "removedApprover",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "RemovedApprover",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "removedOperator",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "RemovedOperator",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "uint256",
          "name": "token0",
          "type": "uint256"
        },
        {
          "indexed": true,
          "internalType": "uint256",
          "name": "token1",
          "type": "uint256"
        },
        {
          "indexed": true,
          "internalType": "bytes32",
          "name": "marketId",
          "type": "bytes32"
        }
      ],
      "name": "TokenRegistered",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "pauser",
          "type": "address"
        }
      ],
      "name": "TradingPaused",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "pauser",
          "type": "address"
        }
      ],
      "name": "TradingUnpaused",
      "type": "event"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "admin_",
          "type": "address"
        }
      ],
      "name": "addAdmin",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "approver_",
          "type": "address"
        }
      ],
      "name": "addApprover",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "operator_",
          "type": "address"
        }
      ],
      "name": "addOperator",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "name": "admins",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "name": "approvers",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order",
          "name": "order",
          "type": "tuple"
        }
      ],
      "name": "cancelOrder",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order[]",
          "name": "orders",
          "type": "tuple[]"
        }
      ],
      "name": "cancelOrders",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "_signer",
          "type": "address"
        },
        {
          "internalType": "address",
          "name": "_proxy",
          "type": "address"
        }
      ],
      "name": "checkProxyWalletAddress",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "domainSeparator",
      "outputs": [
        {
          "internalType": "bytes32",
          "name": "",
          "type": "bytes32"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order",
          "name": "order",
          "type": "tuple"
        },
        {
          "internalType": "uint256",
          "name": "fillAmount",
          "type": "uint256"
        }
      ],
      "name": "fillOrder",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order[]",
          "name": "orders",
          "type": "tuple[]"
        },
        {
          "internalType": "uint256[]",
          "name": "fillAmounts",
          "type": "uint256[]"
        }
      ],
      "name": "fillOrders",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "token",
          "type": "uint256"
        }
      ],
      "name": "getComplement",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "getCurrency",
      "outputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "getFactory",
      "outputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "token",
          "type": "uint256"
        }
      ],
      "name": "getMarketId",
      "outputs": [
        {
          "internalType": "bytes32",
          "name": "",
          "type": "bytes32"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "getMaxFeeRate",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "pure",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "bytes32",
          "name": "orderHash",
          "type": "bytes32"
        }
      ],
      "name": "getOrderStatus",
      "outputs": [
        {
          "components": [
            {
              "internalType": "bool",
              "name": "isFilledOrCancelled",
              "type": "bool"
            },
            {
              "internalType": "uint256",
              "name": "remaining",
              "type": "uint256"
            }
          ],
          "internalType": "struct OrderStatus",
          "name": "",
          "type": "tuple"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "_addr",
          "type": "address"
        }
      ],
      "name": "getSafeAddress",
      "outputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order",
          "name": "order",
          "type": "tuple"
        }
      ],
      "name": "hashOrder",
      "outputs": [
        {
          "internalType": "bytes32",
          "name": "",
          "type": "bytes32"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "incrementNonce",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "usr",
          "type": "address"
        }
      ],
      "name": "isAdmin",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "usr",
          "type": "address"
        }
      ],
      "name": "isApprover",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "usr",
          "type": "address"
        }
      ],
      "name": "isOperator",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "usr",
          "type": "address"
        },
        {
          "internalType": "uint256",
          "name": "nonce",
          "type": "uint256"
        }
      ],
      "name": "isValidNonce",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order",
          "name": "takerOrder",
          "type": "tuple"
        },
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order[]",
          "name": "makerOrders",
          "type": "tuple[]"
        },
        {
          "internalType": "uint256",
          "name": "takerFillAmount",
          "type": "uint256"
        },
        {
          "internalType": "uint256[]",
          "name": "makerFillAmounts",
          "type": "uint256[]"
        }
      ],
      "name": "matchOrders",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "name": "nonces",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        },
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        },
        {
          "internalType": "uint256[]",
          "name": "",
          "type": "uint256[]"
        },
        {
          "internalType": "uint256[]",
          "name": "",
          "type": "uint256[]"
        },
        {
          "internalType": "bytes",
          "name": "",
          "type": "bytes"
        }
      ],
      "name": "onERC1155BatchReceived",
      "outputs": [
        {
          "internalType": "bytes4",
          "name": "",
          "type": "bytes4"
        }
      ],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        },
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        },
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        },
        {
          "internalType": "bytes",
          "name": "",
          "type": "bytes"
        }
      ],
      "name": "onERC1155Received",
      "outputs": [
        {
          "internalType": "bytes4",
          "name": "",
          "type": "bytes4"
        }
      ],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "name": "operators",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "bytes32",
          "name": "",
          "type": "bytes32"
        }
      ],
      "name": "orderStatus",
      "outputs": [
        {
          "internalType": "bool",
          "name": "isFilledOrCancelled",
          "type": "bool"
        },
        {
          "internalType": "uint256",
          "name": "remaining",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "parentCollectionId",
      "outputs": [
        {
          "internalType": "bytes32",
          "name": "",
          "type": "bytes32"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "pauseTrading",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "paused",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "proxyHelper",
      "outputs": [
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "token",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "complement",
          "type": "uint256"
        },
        {
          "internalType": "bytes32",
          "name": "marketId",
          "type": "bytes32"
        }
      ],
      "name": "registerToken",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "",
          "type": "uint256"
        }
      ],
      "name": "registry",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "complement",
          "type": "uint256"
        },
        {
          "internalType": "bytes32",
          "name": "marketId",
          "type": "bytes32"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "admin",
          "type": "address"
        }
      ],
      "name": "removeAdmin",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "approver",
          "type": "address"
        }
      ],
      "name": "removeApprover",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "operator",
          "type": "address"
        }
      ],
      "name": "removeOperator",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "renounceAdminRole",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "renounceOperatorRole",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "_newProxyHelper",
          "type": "address"
        }
      ],
      "name": "setProxyHelper",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "bytes4",
          "name": "interfaceId",
          "type": "bytes4"
        }
      ],
      "name": "supportsInterface",
      "outputs": [
        {
          "internalType": "bool",
          "name": "",
          "type": "bool"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "unpauseTrading",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "token",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "complement",
          "type": "uint256"
        }
      ],
      "name": "validateComplement",
      "outputs": [],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order",
          "name": "order",
          "type": "tuple"
        }
      ],
      "name": "validateOrder",
      "outputs": [],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "bytes32",
          "name": "orderHash",
          "type": "bytes32"
        },
        {
          "components": [
            {
              "internalType": "uint256",
              "name": "salt",
              "type": "uint256"
            },
            {
              "internalType": "address",
              "name": "maker",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "signer",
              "type": "address"
            },
            {
              "internalType": "address",
              "name": "taker",
              "type": "address"
            },
            {
              "internalType": "uint256",
              "name": "tokenId",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "makerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "takerAmount",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "expiration",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "nonce",
              "type": "uint256"
            },
            {
              "internalType": "uint256",
              "name": "feeRateBps",
              "type": "uint256"
            },
            {
              "internalType": "enum Side",
              "name": "side",
              "type": "uint8"
            },
            {
              "internalType": "enum SignatureType",
              "name": "signatureType",
              "type": "uint8"
            },
            {
              "internalType": "bytes",
              "name": "signature",
              "type": "bytes"
            }
          ],
          "internalType": "struct Order",
          "name": "order",
          "type": "tuple"
        }
      ],
      "name": "validateOrderSignature",
      "outputs": [],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "uint256",
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "validateTokenId",
      "outputs": [],
      "stateMutability": "view",
      "type": "function"
    }
  ]
  ```

  </details>

### 2. Documentation

- Storage variables & structs

```js
bytes32 constant ORDER_TYPEHASH = keccak256(
    "Order(uint256 salt,address maker,address signer,address taker,uint256 tokenId,uint256 makerAmount,uint256 takerAmount,uint256 expiration,uint256 nonce,uint256 feeRateBps,uint8 side,uint8 signatureType)"
);

struct Order {
    /// @notice Unique salt to ensure entropy
    uint256 salt;
    /// @notice Maker of the order, i.e the source of funds for the order
    address maker;
    /// @notice Signer of the order
    address signer;
    /// @notice Address of the order taker. The zero address is used to indicate a public order
    address taker;
    /// @notice Token Id of the CTF ERC1155 asset to be bought or sold
    /// If BUY, this is the tokenId of the asset to be bought, i.e the makerAssetId
    /// If SELL, this is the tokenId of the asset to be sold, i.e the takerAssetId
    uint256 tokenId;
    /// @notice Maker amount, i.e the maximum amount of tokens to be sold
    uint256 makerAmount;
    /// @notice Taker amount, i.e the minimum amount of tokens to be received
    uint256 takerAmount;
    /// @notice Timestamp after which the order is expired
    uint256 expiration;
    /// @notice Nonce used for onchain cancellations
    uint256 nonce;
    /// @notice Fee rate, in basis points, charged to the order maker, charged on proceeds
    uint256 feeRateBps;
    /// @notice The side of the order: BUY or SELL
    Side side;
    /// @notice Signature type used by the Order: EOA, PROXY_WALLET or GNOSIS_SAFE
    SignatureType signatureType;
    /// @notice The order signature
    bytes signature;
}

enum SignatureType {
    // 0: ECDSA EIP712 signatures signed by EOAs
    EOA,
    // 1: EIP712 signatures signed by EOAs that own PredictHub Proxy wallets
    PROXY_WALLET,
    // 2: EIP712 signatures signed by EOAs that own PredictHub Gnosis safes
    GNOSIS_SAFE
}

enum Side {
    // 0: buy
    BUY,
    // 1: sell
    SELL
}

enum MatchType {
    // 0: buy vs sell
    COMPLEMENTARY,
    // 1: both buys
    MINT,
    // 2: both sells
    MERGE
}

struct OrderStatus {
    bool isFilledOrCancelled;
    uint256 remaining;
}
```

- Read Functions

- Write Functions

```js
function matchOrders(
        Order memory takerOrder,
        Order[] memory makerOrders,
        uint256 takerFillAmount,
        uint256[] memory makerFillAmounts
    ) external nonReentrant onlyOperator notPaused
```
