Uart interface with adaptive baud rate
Design purpose: To realize arbitrary Uart protocol interface without uniform baud rate
设计目的：不需要统一波特率，实现任意的波特率的Uart协议接口
自适应波特率的uart接口

1.verilog （设计和仿真）
2.自适应波特率  （使用50M的主时钟，可以适应到15M左右）
3.设计思路：假设硬件要处理任意的波特率， 那么达成设定，在uart协议中的开始第一帧8位数据，定义为8bit 0。
4.注意：第一个数据帧按照 1bit起始位+8bit数据0，来考虑设计。




1.verilog (Design and simulation)
2. Adaptive baud rate (using 50M master clock, can be adapted to about 15M)
3. Design idea: Assuming the hardware to process arbitrary baud rate, then reach the setting, the first frame of 8-bit data in the uart protocol is defined as 8bit 0.
4. Note: The first frame is designed according to 1bit starting bit +8bit data 0.
1.verilog (Design and simulation)
2. Adaptive baud rate (using 50M master clock, can be adapted to about 15M)
3. Design idea: Assuming the hardware to process arbitrary baud rate, then reach the setting, the first frame of 8-bit data in the uart protocol is defined as 8bit 0.
4. Note: The first packet is designed according to 1bit starting bit +8bit data 0.