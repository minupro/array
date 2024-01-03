

def bubble(nums):
    lenght = len(nums) - 1
    swap = False
    while not swap:
        swap = True
        for i in range(lenght):
            if nums[i] > nums[i + 1]:
                nums[i], nums[i + 1] = nums[i + 1], nums[i]
                swap = False
    return nums
    
print(bubble([12, 55, 1, 47, 21, 45, 99, 88, 77, 14, 56]))
