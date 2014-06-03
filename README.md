JSON.parseMore
==============

Based on Crockford's json_parse.js, this not eval based JSON parser adds support for the much needed NaN and infinities.

[Test it online](http://dystroy.org/JSON.parseMore)


Why ?
-----

* because when you deal with numbers in a scientific or technical applications, it's hard not to use IEEE754's NaN and sometimes painful not to use infinities
* because some JSON builders let you write NaN (for example Google's gson)
* because `eval('('+json+')')` fails on IE with big JSON strings
    

How to use it ?
---------------

Download the js file and import it :

    <script src=json_parseMore.js></script>

and then parse any JSON string using

    var parsed = JSON.parseMore(json);


License
-------

Public Domain. Use as you wish and at your own risk.
