.. _npm_base32:

npm: @voken/base32
==================

- npm: https://www.npmjs.com/package/@voken/base32
- GitHub: https://github.com/voken1000g/npm-base32
- Toolkit: https://github.com/voken1000g/toolkit/base32


Compute Voken flavored Base32 encoding/decoding, with auto checksum.

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


Install
-------

.. code-block:: bash

   npm i --save @voken/base32

for yarn:

.. code-block:: bash

   yarn add @voken/base32


API
---

encode(input)
_____________

``input`` must be a `Buffer`_ or an ``Array``. Returns a ``String``.

.. _Buffer:
   https://nodejs.org/api/buffer.html

.. code-block:: javascript

   const base32 = require('@voken/base32')

   const bytes = Buffer.from('This is a example.')
   const decoded = base32.encode(bytes)
   console.log(decoded)
   // => AhM6jvS0d5Sj0R90CNV62UbGDHjJV


decode(input)
_____________

``input`` must be a Base32 encoded ``String``. Returns a `Buffer`_.

.. code-block:: javascript

   const base32 = require('@voken/base32')

   const encoded = 'AhM6jvS0d5Sj0R90CNV62UbGDHjJV'
   const bytes = base32.decode(encoded)
   console.log(bytes.toString())
   // => This is a example.


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
