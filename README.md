*** Neural Network *** 
Neural Network with backprop.
Based on very simple explanation and walkthrough by Andrej Karpathy.

Lesson Learned: Make sure your backpropagation callback is properly wired otherwise be ready for countless debugging hour. In my case, gradient was available in non linear operation(tanh/relu) but it did not flowed through addition node i.e., gradient was 0. I had setup callback incorrectly in tanh.
