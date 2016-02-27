# Easiest way to extract unix timestamp in JS

We frequently need to calculate with unix timestamp. There are several ways to grab the timestamp. For current unix timestamp easiest and fastest way is

`const timestamp = Date.now();`

or

`const timestamp = new Date().getTime();`

To get unix timestamp of a specific date pass yyyy-mm-dd as a parameter of Date constructor. For example

`const timestamp = new Date('2012-06-08').getTime()`

You can just add a + sign also when declaring a Date object like below

`const timestamp = +new Date()`

or for specific date

`const timestamp = +new Date('2012-06-08')`