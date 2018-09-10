# compilers
phaedra
source /opt/intel/bin/compilervars.sh 

# Example compiles:

C:	
icc -qopenmp omp_hello.c -o hello
gcc -fopenmp omp_hello.c -o hello
pgcc -mp omp_hello.c -o hello
clang -fopenmp omp_hello.c -o hello

Fortran:	
ifort -qopenmp omp_hello.f -o hello
gfortran -fopenmp omp_hello.f -o hello
pgf90 -mp omp_hello.f -o hello

# Number of threads
bash:
export OMP_NUM_THREADS=$NUMBER
csh:
setenv OMP_NUM_THREADS $NUMBER


