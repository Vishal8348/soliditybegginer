#  Create a Token
We are here  using Solidity  to create a Token.


# Description

This program is written in Solidity. 
Here we created  token with the help of different variables , function, looping statement, and used our learning here that what we studied from our course

 We are using function 
 MINT to  increases the total supply by that number and increases the balance  of the “sender” address by that amount.
                                                      And using
 BURN function that it will then deduct the value from the total supply and from the balance of the “sender”.
 
# Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:

contract MyToken
{
    string public  myTokenName ="Hamp";
    string public  myTokenAbbrv ="Drag";
    uint public  myTokenTotalSupply =0;
    mapping(address =>uint) public amount;
    function mint (address _address , uint _amount) public
    {
      myTokenTotalSupply  += _amount;
      balance[_address] += _amount;
    }
    function burn  (address _address , uint _amount) public 
    {
      if(balance[_address] >= _amount)
      {
      myTokenTotalSupply  -= _amount;
      balance[_address] -= _amount;
      }
    }
}

 We goto "DEPLOY & RUN TRANSACTIONS" and click on Deploy .
 
 Then click on "Deployed/Unpinned Contracts".
 Then we can copy Account id and we do further use of mint and burn function .

 We can also  do check our "Token Name, Token Abbrv., Total Supply " amount there.
## Authors

Vishal Panwar
hunnykanwar2022@gmail.com

## License
This project is licensed under the MIT License - see the LICENSE.md file for detail
