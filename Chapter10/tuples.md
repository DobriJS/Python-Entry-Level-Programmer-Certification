Certified Entry-Level Python Programmer Certification


CHAPTER 10.1
Tuples

The most common immutable sequence type that we're going to work with is going to be the tuple.

Tuples
Tuples are a fixed width, immutable sequence type. We create tuples using parenthesis (()) and at least one comma (,):

>>> point = (2.0, 3.0)

Since tuples are immutable, we don't have access to the same methods that we do on a list. We can use tuples in some operations like concatenation, but we can't change the original tuple that we created:

>>> point_3d = point + (4.0,)
>>> point_3d
(2.0, 3.0, 4.0)

One interesting characteristic of tuples is that we can unpack them into multiple variables at the same time:

>>> x, y, z = point_3d
>>> x
2.0
>>> y
3.0
>>> z
4.0

When we'll most likely to see tuples is while looking at a format string that's compatible with Python 2 (though this will go away soon):

>>> print("My name is: %s %s" % ("Keith", "Thompson"))