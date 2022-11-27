Hello World
===========

Links
-----

-  `catapi's website <https://api.wispace.ru/cat>`__
-  `author's website <https://api.wispace.ru/cat>`__
-  `author's telegram channel <https://t.me/wispace_ru>`__

Quickstart
==========

Using a programming language…

1. Load ``https://api.wispace.ru/cat/api``
2. Get first index from array.
3. Load url from JSON

Code examples
=============

Python
------

.. code:: py

   import requests, webbrowser

   url = requests.get("https://api.wispace.ru/cat/api").json()[0]
   webbrowser.open(url)

JS
--

.. code:: js

   fetch("https://api.wispace.ru/cat/api/").then((response) => {
       return response.json();
   }).then((data) => {
       document.body.innerHTML = "<img src='"+ data[0] +"'></img>"
   })
