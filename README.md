


// SPDX-License-Identifier: MIT
pragma solidity 0.8.19;

contract assignment{
    uint256 result;
    function viewResult() public view returns(uint){
        return result;
    }
    function increment() public returns(uint256) {
        return result++;
    }

    function decrement() public returns(uint256){
        return result--;
    }

    function evenOdd(int _num) public pure returns(string memory){
        if(_num%2 == 0){
            return "Your input was an even number got you sucker....";
        }else{
            return "you entered an odd function........";
        }
    }

    // most significant bit
   
    function mostSignificantBit(uint _x) public pure returns(uint256 _r){
         // x >=2**128
        if(_x >=2**128){
            _x>>=128;
            _r +=128;
        }
         // x >=2**64
        if(_x >=2**64){
            _x>>=64;
            _r +=64;
        }
         // x >=2**32
        if(_x >=2**32){
            _x>>=32;
            _r +=32;
        }
         // x >=2**16
        if(_x >=2**16){
            _x>>=16;
            _r +=16;
        }
         // x >=2**8
        if(_x >=2**8){
            _x>>=8;
            _r +=8;
        }
         // x >=2**4
        if(_x >=2**4){
            _x>>=4;
            _r +=4;
        }
         // x >=2**2
        if(_x >=2**2){
            _x>>=2;
            _r +=2;
        }
         // x >=2**1
        if(_x >=2**1){
            _x>>=1;
            _r +=1;
        }
      
    }
   
}
