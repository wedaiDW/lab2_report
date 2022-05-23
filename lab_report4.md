We use the given markdown file to update our tests, and here are new test files.  
Here is our testfile.  
![](LR4/LR4_omt.png)  
And here is our result:  
![](LR4/LR4_of.png)  
There are some kind of failures in each of the test cases. And we will analyze why these case may fail later in this report.  
Now we need to show the modified testfile and test result for the one we reviewed.  
![](LR4/LR4_tmt.png)  
Test result  
![](LR4/LR4_tf.png)  
### Analysis of failing case and potential improvement  
For the `first case`, both implement runs into the same error, both are not considering the case that is wrapped with \`  
To fix this case, just add a detection method like the one to distinct from image and link and this should pass the test case.  
Then for the `second case`. In this case, although both implement failed with different output, the error is caused by the same mechanism. First of all, both implement failed to solve nested links, however, in outputwise, they are having an output that is closer to expected than ours. This is because in their implementation they are considering line wise rather than whole file. To fix this is more complicated than just few lines of code, because the nested link have a specific order of which link is to be render as a link. The implement will have to match the parentheses while matching the correct link.  
The `third case` is different, it has different output with different mechanism causing this error. For our code, this is caused by the matching of parentheses and nested link
