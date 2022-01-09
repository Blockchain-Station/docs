# Create a Variable-cap Asset

## Create the Asset

### 1. Write the token smart contract

{% embed url="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol" %}

{% hint style="info" %}

{% endhint %}

#### Functions

* name()
* symbol()
* decimals()
* totalSupply()
* balanceOf(account)
* transfer(recipient, amount)
* allowance(owner, spender)
* approve(spender, amount)
* transferFrom(sender, recipient, amount)
* increaseAllowance(spender, addedValue)
* decreaseAllowance(spender, subtractedValue)
* \_transfer(sender, recipient, amount)
* \_mint(account, amount)
* \_burn(account, amount)
* \_approve(owner, spender, amount)
* \_setupDecimals(decimals\_)

### 2. Compile your code into bytecode

### 3. Deploy your Variable-cap Asset by sending your code in a transaction to the Enter network

### 4. Navigate to[ the explorer](https://scantest.entercoin.net) to check that your token has been created

### 5. **You can use the \_mint function to create additional units of the token**