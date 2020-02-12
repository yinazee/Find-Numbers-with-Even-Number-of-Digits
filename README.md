# Find-Numbers-with-Even-Number-of-Digits
Leetcode Challenge Javascript


Solution:

// nums = [12,345,2,6,7896]
// nums = ["12","345","2","6","7896"]
// nums = [2, 3, 1, 1, 4]
// nums = [2,4]
// nums.length = 2
// output = 2

let findNumbers = function(nums) {
    let count = 0
    for (let i = 0; i < nums.length; i++) {
        count += nums[i].toString().length % 2 ? 0 : 1
    }
    return count
};
