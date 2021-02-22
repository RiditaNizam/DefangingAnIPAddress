# DefangingAnIPAddress
Leetcode Easy 1108

Given a valid (IPv4) IP address, return a defanged version of that IP address.

A defanged IP address replaces every period "." with "[.]".

class Solution:
    def defangIPaddr(self, address: str) -> str:

        answerString = ""
        
        for character in address:
            if character == ".":
                answerString += "[.]"
            else:
                answerString += character
        return answerString
