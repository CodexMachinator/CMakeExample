# Build
cd build;
cmake .. -DCMAKE_BUILD_TYPE=Debug -G "Unix Makefiles"; make

# Outputs
./src/example_run
./tst/example_tst

# Clean up
make clean; rm -rf *; rm -rf ../lib/googletest/g* *
