.. _npm_address:

npm: @voken/address
===================

- npm: https://www.npmjs.com/package/@voken/address
- GitHub: https://github.com/voken1000g/npm-address

Covert a public key to Voken wallet address. Or verify an address.


Install
-------

.. code-block:: bash

   npm i --save @voken/address

for yarn:

.. code-block:: bash

   yarn add @voken/address


API
---

fromPublicKey(input)
____________________

``input`` must be a `Buffer`_. Returns a ``String``.

.. _Buffer:
   https://nodejs.org/api/buffer.html

.. code-block:: javascript

   const vokenAddress = require('@voken/address')

   const bytes = Buffer.from('02038de5ca300de53a6bc109c7178d4cb4d0cb626ff824c03872c64291fd04d8fa', 'hex')
   const address = vokenAddress.fromPublicKey(bytes)
   console.log(address)
   // => vbnjAa398KKqj6YJ174EMCAWn1ku3tnF5


isAddress(input)
________________

``input`` must be a ``String``. Returns ``true`` if ``input`` is a valid Voken wallet address.

.. code-block:: javascript

   const vokenAddress = require('@voken/address')

   console.log(vokenAddress.isAddress('vMN296Q5B54j49n8Wdq4RYrsEhYm9aNDx'))
   // => true
   console.log(vokenAddress.isAddress('v74NJWe7hjs5H3n87K4A97tK8NkPXya6T'))
   // => true
   console.log(vokenAddress.isAddress('vJK2QHmmpaNU3BvP4D5K4cKm5Gf8E2Jjk'))
   // => true

   console.log(vokenAddress.isAddress('v6U27674GH4Qb3Cav29PYbYW16f0HeT090'))
   // => false
   console.log(vokenAddress.isAddress('v6U27674GH4Qb3Cav29PYbYW16f0HeT0'))
   // => false
   console.log(vokenAddress.isAddress('i6U27674GH4Qb3Cav29PYbYW16f0HeT09'))
   // => false
   console.log(vokenAddress.isAddress('v6U27674GH4Qb3Cav29PYbYW16f0Het09'))
   // => false


Hack / Test
-----------

Uses JavaScript standard style. Read more:

|js-standard-style|_


.. |js-standard-style| image:: https://cdn.rawgit.com/feross/standard/master/badge.svg
.. _js-standard-style:
   https://github.com/feross/standard


Credits
-------

- `Mike Hearn`_ for original Java implementation
- `Stefan Thomas`_ for porting to JavaScript
- `Stephan Pair`_ for buffer improvements
- `Daniel Cousens`_ for cleanup and merging improvements from bitcoinjs-lib
- `Jared Deckard`_ for killing ``bigi`` as a dependency


.. _Mike Hearn:
   https://github.com/mikehearn
.. _Stefan Thomas:
   https://github.com/justmoon
.. _Stephan Pair:
   https://github.com/gasteve
.. _Daniel Cousens:
   https://github.com/dcousens
.. _Jared Deckard:
   https://github.com/deckar01


License
-------

MIT
