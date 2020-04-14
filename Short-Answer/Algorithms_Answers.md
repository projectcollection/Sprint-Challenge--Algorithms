Add your answers to the Algorithms exercises here.

I
a: O(n^3)

b: O(9n^4 - 36n^3 - 18n^2 + 72n) -> O(n^4)

c: O(n)

II

heights_to_consider = [0,n]

drop an egg at (heights_to_consider[1]-heights_to_consider[0])//2
	if egg breaks then heights_to_consider[1] = n//2
	else heights_to_consider[0] = n//2
repeat until the difference for htc[1]-htc[0] = 1

test a drop at htc[1]
	if breaks then f = htc[0]
	else f = htc[1]
