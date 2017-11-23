NOTE:
THIS IS A MODIFIED VERSION OF RRR
http://github.com/ylatif/g2o

suitesparse:

  - sudo apt-get install libsuitesparse-dev

cmake 3:

  - sudo apt-get install software-properties-common
  - sudo add-apt-repository ppa:george-edison55/cmake-3.x
  - sudo apt-get update 

g2o:

  - git clone https://github.com/RainerKuemmerle/g2o
  - cd g2o
  - mkdir build
  - cd build
  - cmake ..
  - make
  - sudo make install

build

  - cd rrr
  - mkdir build <br>
  - cd build <br>
  - cmake .. <br>
  - make <br>
 
  This will generate examples in the folder rrr/build/examples/
  
Running the examples

  ./build/examples/RRR\_3D\_from\_disk\_g2o data\_error.g2o 70

After running RRR, run g2o
  - ~/g2o/bin/g2o -o out.g2o data\_error.g2o

out.g2o is the final file.
