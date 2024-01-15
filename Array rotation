# Python program to left-rotate the given array

# Function reverse the given array
# by swapping first and last numbers.


def reverse(start, end, arr):

	# No of iterations needed for reversing the list
	no_of_reverse = end-start+1

	# By incrementing count value swapping 
	# of first and last elements is done.
	count = 0
	while((no_of_reverse)//2 != count):
		arr[start+count], arr[end-count] = arr[end-count], arr[start+count]
		count += 1
	return arr

# Function takes array, length of
# array and no of rotations as input


def left_rotate_array(arr, size, d):

	# Reverse the Entire List
	start = 0
	end = size-1
	arr = reverse(start, end, arr)

	# Divide array into twosub-array
	# based on no of rotations.
	# Divide First sub-array
	# Reverse the First sub-array
	start = 0
	end = size-d-1
	arr = reverse(start, end, arr)

	# Divide Second sub-array
	# Reverse the Second sub-array
	start = size-d
	end = size-1
	arr = reverse(start, end, arr)
	return arr


arr = [1, 2, 3, 4, 5, 6, 7, 8]
size = 8
d = 1
print('Original array:', arr)

# Finding all the symmetric rotation number
if(d <= size):
	print('Rotated array: ', left_rotate_array(arr, size, d))
else:
	d = d % size
	print('Rotated array: ', left_rotate_array(arr, size, d))

