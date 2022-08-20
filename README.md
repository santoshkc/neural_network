# Neural Network with Backprop

**Based on very simple explanation and walkthrough by Andrej Karpathy.**

**Lesson Learned**: Make sure your back propagation callback is properly wired otherwise be ready for countless debugging hour. 
In my case, gradient was available in non linear operation(**tanh/relu**) but it did not flowed through addition node i.e., gradient was 0.0. I had setup callback incorrectly in tanh. 
Visualization helped to highlight underlying issue quickly. However, I could not find out exact cause. 
