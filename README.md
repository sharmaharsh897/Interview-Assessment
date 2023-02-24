# Interview-Assessment

Q1. Middle of Three

BasicAccuracy: 54.8%Submissions: 64K+Points: 1

Given three distinct numbers A, B and C. Find the number with value in middle (Try to do it with minimum comparisons).
 Example 1:
Input: A = 978, B = 518, C = 300 Output: 518 Explanation: Since 518>300 and 518<978, so 518 is the middle element.  
SOLUTION   class Solution{
    middle(A, B, C){
        //code here
        let arr=[]
        arr.push(A,B,C)
        arr = arr.sort(function(a,b) {return a-b})
        return arr[1]
    }
}




Q2. Display longest name

SchoolAccuracy: 66.29%Submissions: 48K+Points: 0

Given a list of names, display the longest name.
 Example:
Input: N = 5 names[] = { "Geek", "Geeks", "Geeksfor", "GeeksforGeek", "GeeksforGeeks" } Output: GeeksforGeeks

SOLUTION:

class Solution {

    longest(names,n){
        //code here
        let high=0;
        let s=0;
        for(let i=0;i<names.length;i++){
            if(names[i].length>high){
                high=names[i].length
                s=i
            }
            
        }
        return names[s];
    }
}





Q3. Replace all 0's with 5

BasicAccuracy: 75.55%Submissions: 62K+Points: 1

You are given an integer N. You need to convert all zeroes of N to 5.
Example 1:
Input: N = 1004 Output: 1554 Explanation: There are two zeroes in 1004 on replacing all zeroes with "5", the new number will be "1554".  SOLUTION:

 class Solution {
    
    convertFive(num)
    {
       return num.toString().split('').map(d=>d==='0' ?'5':d).join('');
    }
    
}