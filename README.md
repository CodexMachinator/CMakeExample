# Build
cd build
cmake .. -DCMAKE_BUILD_TYPE=Debug -G "Unix Makefiles" 
make

# Outputs
./src/helloci_run
./tst/helloci_tst

# Clean up
make clean
rm -rf *
rm -rf ../lib/googletest/g* *
