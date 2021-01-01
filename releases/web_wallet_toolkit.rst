.. _web_wallet_toolkit:

Voken HD Wallet Generator/Validator
===================================

- HD Wallet Generator: https://voken1000g.github.io/toolkit/wallet-generator
- HD Wallet Validator: https://voken1000g.github.io/toolkit/wallet-validator
- GitHub: https://github.com/voken1000g/toolkit


BIP39 mnemonic
--------------

Mnemonic code for generating deterministic keys

`BIP39`_: A group of easy to remember words -- for the generation of deterministic wallets.

.. _BIP39:
   https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki


BIP32 HD Wallet
---------------

Hierarchical Deterministic Wallets

`BIP32`_: Use the binary seed converted from a BIP39 mnemonic to generate hierarchical deterministic wallets.

.. _BIP32:
   https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki


BIP44 Multi-Account
-------------------

Multi-Account Hierarchy for Deterministic Wallets

Voken was listed in `SLIP-0044`_, with ``678`` as the ``coin_type`` value.

Its ``rootPath`` of **BIP44** is ``m/44'/678'/0'/0/...``

Read more at `BIP44`_

.. _SLIP-0044:
   https://github.com/satoshilabs/slips/blob/master/slip-0044.md

.. _BIP44:
   https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki


Native checksum
---------------

A valid voken wallet address looks like: ``v8TX860N7Eu1jMv1yQJkb8fykXts2mVAG``

It is a native checksum address.
Any misspelling of even a single character will fail in address verification.
This means that no Voken will be lost due to someone mistyped/pasted an wrong address.


ALPHABET for @voken/base32
--------------------------

`@voken/base32` is human-friendly --
you don't have to worry about letters/numbers that are easy to confuse,
making it easier to transmit in handwriting or typing over the phone.

The encoding alphabet consists of the numerals ``0-9`` and the letters ``a-z``,
excluding a few letters that might look like numbers,
which we simply interpret as follows:

- ``i``, ``l`` -> ``1``
- ``o`` -> ``0``
- ``z`` -> ``2``

.. code-block:: javascript

   const ALPHABET = '0123456789abcdefghjkmnpqrstuvwxy'


Each character corresponds to 5 bits of input.

Lexicographic order of strings is preserved through Base 32 encoding.


Packages in NPM
---------------

- :ref:`npm_hd_wallet`
- :ref:`npm_address`
- :ref:`npm_base32`
- :ref:`npm_avatar`
- :ref:`npm_private_key`
- :ref:`npm_public_key`
