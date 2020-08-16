```
temp=input('Enter an int >0.     ')
n=int(temp)
count=0

def fib(n):
    '''Assumes that n is an int >=0,
		returns the fibnacci result.'''

		global count
		count+=1
		if n==0 or n==1:
   	 	return 1
		return fib(n-1)+fib(n-2)

print(fib(n))
print(count)
```

