# Lobanov Ivan
## Contacts:
> Phone number: +7(931)-402-71-44  
> Email: [asdnbvb123@gmail.com](asdnbvb123@gmail.com)
## About myself.
Currently on my third year in ITMO University, under specialization of "Developing of graphic and web applications". I am highly interesterd in web development, and since November learning in this field. Currently finishing learning React. After that I want to test developing apps with Next.js and React Query. Very curious about blockchain development, would like to learn Rust and read more about smart-contracts. Opened to job proposals in field of frontend development. Despite I might not have any commertial expirience, I believe myself as a fast learner and expirienced in theoretical field.
## Skills
### Hard Skills
> Java, HTML, CSS, JavaScript, React, Redux, Git, Material UI, Chakra UI.
### Soft Skills
>Fast learning, working in a team, time-management. 
## Code Example
> Task "Maximum Perimeter Triangle" from [hackerranl.com].
Task description: 
*
Given an array of stick lengths, use 3 of them to construct a non-degenerate triangle with the maximum possible perimeter. Return an array of the lengths of its sides as 3 integers in non-decreasing order.  
If there are several valid triangles having the maximum perimeter:  
1. Choose the one with the longest maximum side.  
2. If more than one has that maximum, choose from them the one with the longest minimum side.  
3. If more than one has that maximum as well, print any one them.  
If no non-degenerate triangle exists, return [-1].
*
```
function maximumPerimeterTriangle(sticks) {
    // Write your code here
    let output = 0;
    let max = [-1];
    sticks.sort((a, b) => a - b);
    
    for(let i = sticks.length; i >= 2; i--) {
        for(let j = i - 1; j >= 1; j--)
            for(let k = i - 2; k >= 0; k--) {
                if(sticks[j] + sticks[k] > sticks[i] &&
                sticks[j] + sticks[k] + sticks[i] > max) {
                    max = [sticks[k], sticks[j], sticks[i]]
                }
            }
    }
    
    return max == [-1] ? -1 : max;
}
```
## Job Expirience 
When I studied "Front-End Web Development with React" on Coursera, I used to work with React, Redux, React-Router, Webpack. It resulted in application, that have a description of local Indian food recipes, as well as some forms to leave comments on this concrete dishes. 
## Education
> Coursera: "Front-End Web Development with React"  
> OpenEdu: "Algorythms and Data Structures"
## Degree
Bachelor degree in Computer Science, 2023.
## Languages
Russian: native.  
English: B2.
