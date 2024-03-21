### Post-fix algorithm

1. if input is operand output it
2. if input is operator

a. if stack is empty oOT topo of stack is (OR input > Top of stack push input in stack)

b. else pop all item in the stack with presence >= input and place title in output. stop if(is encountered)

3. if input is(push it in the stack) 4. if input is pop all items and place them in the output, stop when you encount and discent 5. at end pop all removing operators in the stack and add them to output

```cpp
if item operand
    push on stack
if item is operator
    poped 2 operands
    apply operator and
    push result on stack

```
