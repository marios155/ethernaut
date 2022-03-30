In solidity, for a contract to be able to receive ether, the fallback function must be marked `payable`.

However, there is no way to stop an attacker from sending ether to a contract by self destroying. Hence, it is important not to count on the invariant `address(this).balance == 0` for any contract logic.

By completing this level, you have gained valuable insight into how a smart contract implements a transcation, and how this implementation can be abused. Your flag is `PaymentsMustBeProtected`.
