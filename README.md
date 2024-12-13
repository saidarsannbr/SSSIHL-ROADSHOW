# SSSIHL-ROADSHOW
Main Code: Output 0
#include<stdio.h>
int main(){
    int sum = 0, i, n;
    printf("Enter the value of n = ");
    scanf("%d",&n);
    for(i = 1;i <= n;i++){
       sum = sum + i;
    }
    printf("The Sum of numbers from 1 to %d is %d\n",n,sum);
    return 0;
}

# Gcc, Instruction set/Architecture,Preperation,Sum,Interactive.

cd Desktop/work/tools/openlane_working_dir/openlane
docker

# Floor Planning, Synthesis, Placement, Routing, Blinking, PWM Fading.

./flow.tcl -interactive

package require openlane 0.9

run_placement

prep -design picorv32a

run_synthesis

run_floorplan

eog designs/picorv32a/runs/13-12_07-

00/results/floorplan/picorva32a.floorplan.def.png

run_placement

eog designs/picorv32a/runs/13-12_07-

00/results/placement/picorva32a.placement.def.png

run_cts

run_routing

Blinking and PWM Fading
