# 8-bit-Dadda-Multiplier
8 X8 Dadda multiplier implemented in Verilog. Dadda multiplier is used for fast multiplication. Dadda multipliers plan on reducing the final number of wires for any weight to 2 with as few and as small adders as possible.We determine the number of layers required first, beginning from the last layer, where no more than 2 wires should be left. We work back from the final adder to earlier layers till we find that we can manage all wires generated by the partial product generator. We know that the final adder can take no more than 2 wires for each weight.Let dj represent the maximum number of wires for any weight in layer j, where j = 1 for the final adder. (Thus d1 = 2). The maximum number of wires which can be handled in layer j+1 (from the end) is the integral part of 3/2 dj . We go up in j, till we reach a number which is just greater than or equal to the largest bunch of wires in any weight.The number of reduction layers required is this jfinal − 1.At each layer we know the maximum number of wires which should be left for the next layer.For each weight, we place the least number of smallest adders, such that the wires going out to the next layer do not exceed the maximum number of wires it can handle.At each weight, we must consider all the sum and pass through wires at this weight, as well as the wires which will be transferred through carry of the less significant weights, to the next layer. That is why we must begin with the lowest weight and go towards higher weights in each layer. 
# Verilog Result
![alt text](https://github.com/Anshul380/8-bit-Dadda-Multiplier/blob/main/Screenshot%202023-08-13%20003247.png?raw=true)

# Layout On Qflow
![alt text](https://github.com/Anshul380/8-bit-Dadda-Multiplier/blob/main/Screenshot%202023-08-13%20003906.png?raw=true)


# Working
![alt text](https://github.com/Anshul380/8-bit-Dadda-Multiplier/blob/main/WhatsApp%20Image%202023-08-13%20at%2001.32.00.jpg?raw=true)


   
