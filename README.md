# CUDAResearch

Modify `second.cu` to go column-by-column instead of row-by-row in the code. That is, the threads blocks should have Dim.x = 1, Dim.y = 512 for example, but you still use the same computation (threadsPerRow * row + col) to compute the thread's index in the array.
* Analyze the performace (using "time" in the shell)
* Read the Cuda C++ Programming Guide to find out why the performance dropped off so badly. (Hint, coalescing.)
