### 1. Contract address

- [0x76eEd609B47d0a986dA28ab7f817D5abB4C3CA79](https://explorer.zksync.io/address/0x76eEd609B47d0a986dA28ab7f817D5abB4C3CA79)
  <details>
    <summary>Abi</summary>

  ```json
  [
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "internalType": "address",
          "name": "value",
          "type": "address"
        }
      ],
      "name": "AdminUpdated",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "internalType": "address",
          "name": "value",
          "type": "address"
        }
      ],
      "name": "AgentFiUpdated",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "internalType": "uint8",
          "name": "version",
          "type": "uint8"
        }
      ],
      "name": "Initialized",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "staker",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "userStaked",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "changeAmount",
          "type": "uint256"
        },
        {
          "indexed": false,
          "internalType": "bool",
          "name": "inceaseOrDecrease",
          "type": "bool"
        }
      ],
      "name": "NotifyBalanceChange",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "previousOwner",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "newOwner",
          "type": "address"
        }
      ],
      "name": "OwnershipTransferred",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "internalType": "address",
          "name": "token",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "amount",
          "type": "uint256"
        }
      ],
      "name": "TokenDistributed",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "internalType": "address",
          "name": "token",
          "type": "address"
        },
        {
          "indexed": true,
          "internalType": "address",
          "name": "user",
          "type": "address"
        },
        {
          "indexed": false,
          "internalType": "uint256",
          "name": "amount",
          "type": "uint256"
        }
      ],
      "name": "TokenHarvested",
      "type": "event"
    },
    {
      "inputs": [],
      "name": "PERCENTAGE_BASE",
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
      "name": "accTokenPerStakedToken",
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
      "name": "admin",
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
      "name": "aigentFi",
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
          "name": "",
          "type": "uint256"
        }
      ],
      "name": "aigentFiTokens",
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
      "name": "countTokens",
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
          "name": "_token",
          "type": "address"
        },
        {
          "internalType": "uint256",
          "name": "_amount",
          "type": "uint256"
        }
      ],
      "name": "distributeRewardAgentFiToken",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "harvest",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "hsStaking",
      "outputs": [
        {
          "internalType": "contract HSStakingInterfaceV6_3",
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
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "name": "indexOfAIgentFiToken",
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
      "name": "initialize",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "contract HSStakingInterfaceV6_3",
          "name": "_hsStaking",
          "type": "address"
        }
      ],
      "name": "initializeV2",
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
      "name": "isActive",
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
          "name": "_staker",
          "type": "address"
        },
        {
          "internalType": "uint256",
          "name": "_stakingAmount",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "_changeAmount",
          "type": "uint256"
        },
        {
          "internalType": "bool",
          "name": "_isIncrease",
          "type": "bool"
        }
      ],
      "name": "notifyBalanceChange",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "owner",
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
          "internalType": "address",
          "name": "_token",
          "type": "address"
        },
        {
          "internalType": "address",
          "name": "_sender",
          "type": "address"
        }
      ],
      "name": "pendingRewardToken",
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
      "name": "renounceOwnership",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "_value",
          "type": "address"
        }
      ],
      "name": "setAdmin",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "internalType": "address",
          "name": "_value",
          "type": "address"
        }
      ],
      "name": "setAgentFi",
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
      "name": "totalRewardsDistributedToken",
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
          "name": "newOwner",
          "type": "address"
        }
      ],
      "name": "transferOwnership",
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
        },
        {
          "internalType": "address",
          "name": "",
          "type": "address"
        }
      ],
      "name": "users",
      "outputs": [
        {
          "internalType": "uint256",
          "name": "debtToken",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "harvestedRewardToken",
          "type": "uint256"
        },
        {
          "internalType": "uint256",
          "name": "pendingRewardToken",
          "type": "uint256"
        }
      ],
      "stateMutability": "view",
      "type": "function"
    }
  ]
  ```

  </details>

### 2. Documentation

- Storage variables

```js
  uint256 public countTokens; //total available tokens
  address[] public aigentFiTokens; //list of tokens
  mapping(address => uint256) public accTokenPerStakedToken; //accumulate to cal reward
  mapping(address => uint256) public totalRewardsDistributedToken; //total reward distributed of token
  mapping(address => bool) public isActive; // token address => isActive

  mapping(address => uint256) public indexOfAIgentFiToken; // token address => index

  mapping(address => mapping(address => User)) public users; // token => user address => info
  //user struct
  struct User {
    uint256 debtToken; // 1e18
    uint256 harvestedRewardToken; // 1e18
    uint256 pendingRewardToken; // 1e18
  }
```

- Functions

  For client-side integration, you can loop **_from 0 to countTokens_** and call get **_aigentFiTokens(i)_**. A more optimized approach is to use multicall.

```js
  function distributeRewardAgentFiToken(address _token, uint256 _amount)
```

The distributeRewardAgentFiToken can only be called from partnerStakingAigentFi to distribute rewards for the tokens.

```js
  function pendingRewardToken(address _token, address _sender)
```

Function pendingRewardToken is used to calculate the reward amount for a specific token of a user. In the future, we will develop a function to retrieve rewards for all tokens belonging to each user.

```js
 function harvest(address[] calldata _tokens)
```

The harvestRewardToken function takes specific tokens as input to be harvested. Currently, it cannot process "harvest all" due to a bug on the partner side, which prevents the transfer of tokens in bonding curves. Once the system is stable, the "harvest all" functionality will be enabled.

```js
 function users(address token, address staker) view returns (User memory)
```

Read infomation of a staker depend on token address

- Events

```js
  event AdminUpdated(address value);
  event AgentFiUpdated(address value);
  event TokenDistributed(address token, uint256 amount);
  event TokenHarvested(address indexed token, address indexed user, uint256 amount);
  event NotifyBalanceChange(address indexed staker, uint256 userStaked, uint256 changeAmount, bool inceaseOrDecrease);
```
