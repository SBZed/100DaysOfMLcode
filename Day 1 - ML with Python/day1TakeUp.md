>>> type(None) #None signifies 'no value' or 'empty value'
Output : <class 'NoneType'>

# Print the current time in seconds (starting from January 1, 1970)
>>> import datetime as dt
>>> import time as tm
>>> tm.time() #print current time in seconds from January 1, 1970
1533370235.0210752

# convert timestamp to datetime
>>> dtnow = dt.datetime.fromtimestamp(tm.time()) 
>>> dtnow.year
Output : 2018

>>> today = dt.date.today()
>>> today
Output : datetime.date(2018, 8, 4)

# Subtract 100 days from today’s date
>>> delta = dt.timedelta(days=100)
>>> today - delta
Output : datetime.date(2018, 4, 26)

# If the sequences used in the zip function is unequal, the returned list is truncated in length to the length of the shortest sequence.

>>> a = [1,2] #create two lists
>>> b = [5,6,7,8]
>>> c = zip(a,b) #Use the zip function
>>> print(c)
Output : [(1,5), (2,6)]

