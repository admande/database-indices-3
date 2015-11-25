#Question 1#

```
EXPLAIN ANALYSE
SELECT * FROM ingredients
WHERE name = 'Brussels sprouts';
```
![before](http://imgur.com/yOaK3jt)
![after](http://imgur.com/X0ZMkL6)
#Question 2#

```
EXPLAIN ANALYSE
SELECT count(*) FROM ingredients
WHERE name = 'Brussels sprouts';
```
![before](http://imgur.com/SXSu6z1)
![after](http://imgur.com/5v1RIu8)
#Question 3#

```
EXPLAIN ANALYSE
SELECT * FROM ingredients
WHERE name = 'Brussels sprouts' AND unit = 'gallon(s)';
```
![before](http://imgur.com/ZqGnNgC)
![after](http://imgur.com/Lz2GsnA)
#Question 4#
```
EXPLAIN ANALYSE
SELECT * FROM ingredients
WHERE name = 'Brussels sprouts' OR name LIKE '%j%' OR unit = 'gallon(s)';
```
![before](http://imgur.com/X0ZMkL6)
![after](http://imgur.com/Pyrmkqs)
#Create an index#

`CREATE INDEX ON ingredients(name);`
