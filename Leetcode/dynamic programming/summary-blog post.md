Consider a problem: [leetcode 53](https://leetcode-cn.com/problems/maximum-subarray/)

## What is dynamic Programming - the basics

### what is the technique 

### when to apply

## On a specific problem

### state relationship
#### naive approach
$$\begin{align}\text{maxsum}(i,j)=\max(\text{maxsum}(i+1,j),\text{maxsum}(i+1,j)+A[i],\\ \text{maxsum}(i,j-1),\text{maxsum}(i,j-1)+A[j])\end{align}$$
where $\text{maxsum}(i,j)$ stands for maximum sum of subarrays between $i$ and $j$.

#### a better one
$$\text{maxsum}(i)=\text{maxsum}(i-1)+A[i]
$$
where $\text{maxsum}(i)$ stands for maximum sum of subarrays end at $i$.