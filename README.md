# clock_gen

`timescale 1ns / 1ps

module clk_gen(clk);
output reg clk;
initial 
clk=1'b0;
always
#5 clk=~clk;
initial
#100 $finish;
endmodule
