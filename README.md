// **** PicoRv32 & Spike co-simulation testbench *** *//

// **** Pre-requisite **** //
1. Install below tools
- GNU Toolchain
  Site : https://github.com/riscv-collab/riscv-gnu-toolchain.git 
- Spike
  Site : https://github.com/riscv-software-src/riscv-isa-sim.git 
- PK(Proxy Kernel)
  Site : https://github.com/riscv-software-src/riscv-pk.git
- Iverilog 
  Site : https://github.com/steveicarus/iverilog.git
- Verilator 
  Site : https://github.com/verilator/verilator.git 

// **** Process **** //
  1. git clone https://github.com/bobj123/RISCV_EX.git
  2. source env.sh
     - Must set the below variable for right path.
       **export RISCV_GNU_TOOLCHAIN_INSTALL_PREFIX=/opt/riscv**
  3. make build2
     - Compilation & Linking
  4. make libspikeso
     - To make shared object to use Spike with VPI
  4. make sim
     - Run simulation and check the log results.
