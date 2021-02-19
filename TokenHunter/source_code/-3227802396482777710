/**
Author: Loopring Foundation (Loopring Project Ltd)
*/

pragma solidity ^0.5.11;


library Cloneable {
    function clone(address a)
        external
        returns (address)
    {

    
        address retval;
        assembly{
            mstore(0x0, or (0x5880730000000000000000000000000000000000000000803b80938091923cF3 ,mul(a,0x1000000000000000000)))
            retval := create(0,0, 32)
        }
        return retval;
    }
}