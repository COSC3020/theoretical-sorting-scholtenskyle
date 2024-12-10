# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

Assuming this could be sorted in O(n) time, we can actually measure it quite easily since the time it takes would just grow linearly. We could give it different sized lists, with different values, and even maybe pre-sorted to different extents. Creating as much variation in these tests would be key. But it would also be very important to keep some things consistent, such as the machine it is run on, and limit background processes. Then we would need to time these tests, and run each one multiple times. With this, we can be sure that we are actually collecting reasonable data. Once this is done we can compare the data sets and see if it does indeed grow linearly consistently.

In class we saw that the complexity of a sorting algorithm was O(nlogn). This is true when doing comparison based sorting, such as when sorting a tree, and deciding which leaf to move to. Of course if there is an array of size n, there are n! leaves in the tree. And of course n! is larger than n in most cases. This means it couldn't possibly go through every value in n time, except in very rare cases (such as if the tree is empty, or only one value). This means that X is not possible.

I just had to revisit the slides to remind myself of how this worked.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
