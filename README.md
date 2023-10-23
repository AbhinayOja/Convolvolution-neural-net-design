
# Convolvolution-neural-net-design
![Gif of my design](https://github.com/AbhinayOja/Convolvolution-neural-net-design/blob/main/Convolution_MaxPooling.gif)

[ Report ](https://github.com/AbhinayOja/Convolvolution-neural-net-design/blob/main/Efficient%20Systolic%20Array%20Convolution%20with%20Pipelined%20MaxPooling%20and%20ReLU%20(1).pdf)


Designed a systolic array-based Convolver, carefully optimizing its pipeline for 1-cycle output when fully loaded.
Additionally, developed a pipelined Maxpooler, that seamlessly integrates with the convolver without impeding its performance, and utilized ReLU activation at the output of Maxpooler.
This pipeline architecture ensures a 1 cycle valid output for the entire Convolver + Maxpooler + ReLU processing,with the final result emerging only 2 cycles after the last input is fetched.
For an NxN input matrix, it takes 2N + 3 cycles to load the convolver and 3N + 4 cycles to load the entire Convolver + Maxpooler + ReLU pipeline.
Outperformed 400 classmates by achieving the class’s lowest clock cycle count.
