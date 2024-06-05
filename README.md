# two_sum2
class Solution:
    numbers = list(map(int, input("enter numbers:").split()))
    target = int(input("enter target:"))
    def two_sum(numbers, target):
        l, r = 0 ,len(numbers)-1

        while l<r:
            poi_sum = numbers[l] + numbers[r]

            if poi_sum > target:
                r = r-1
            elif poi_sum < target:
                l = l+1
            else:
                return[l+1, r+1]
            
    
    print(two_sum(numbers, target))



    

