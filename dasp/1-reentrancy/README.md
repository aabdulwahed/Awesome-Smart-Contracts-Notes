# Reentrancy Attack

#### Definition



#### Code Examples:

   - [Transfer Ether](contracts/TransferEth.sol)
        - [Attacking Transfer Ether](contracts/AttackTransferEth.sol)
        - [Fix Transfer Ether](contracts/GoodTransferEth.sol)
   - [DAO Contract]()
   
#### Quick start
##### 1. starting TestNet

Open a new terminal in order to start start `ganache-cli`. 

```bash
    $ ganache-cli
```

##### 2. Using terminal 2 
install, compile and migrate the following contracts
```bash
    $ npm install
    $ npm run compile
    $ npm run migrate 
```

#### 3. Run attacks

```
    $ turffle test
```

```bash
 Contract: AttackTransferEth
    Test Reentrancy Attack of Bad Transfer Ether Contract
         > Count:  1 Attacker Contract Balance: 500000000000000000
         > Count:  2 Attacker Contract Balance: 1000000000000000000
         > Count:  3 Attacker Contract Balance: 1500000000000000000
         > Count:  4 Attacker Contract Balance: 2000000000000000000
         > Count:  5 Attacker Contract Balance: 2500000000000000000
      ✓ Should able to attack the transfer ether contract (65ms)

```

### References:
- [Solidity Documentation: Reentrancy](https://solidity.readthedocs.io/en/develop/security-considerations.html#re-entrancy)
- [Fallback functions and the fundamental limitations of using send() in Ethereum & Solidity](https://github.com/ConsenSys/Ethereum-Development-Best-Practices/wiki/Fallback-functions-and-the-fundamental-limitations-of-using-send%28%29-in-Ethereum-&-Solidity)
- [Ethereum Blogpost Smart Contract Security](https://blog.ethereum.org/2016/06/10/smart-contract-security/)

