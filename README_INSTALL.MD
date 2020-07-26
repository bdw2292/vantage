
## Pymol Installation
* Download free student education version or paid version through https://pymol.org/

## Download Interface
* git clone 

## Download Poltype
* git clone -b poltype2 git@github.com:pren/poltype.git poltype-poltype2
* Navigate to Examples/SymmetryMethylamine and download the folder

## Windows Tinker Binary Installation:

* Download Excutables in ZIP folder from https://dasher.wustl.edu/tinker/
* Unzip the folder
* Save the path to the tinker bin folder (C:\Users\brand\Desktop\bin-windows-8.7.2\bin-windows\ )
* Copy text file from https://dasher.wustl.edu/tinker/distribution/params/amoebabio18.prm  and save in file called amoebabio18.prm
* Save path from amoebabio.prm in a text file, "C:\Users\brand\Desktop\bin-windows-8.7.2\amoebabio18.txt"

##  Linux Tinker CPU Installation
```
git clone git@github.com:TinkerTools/Tinker.git tinker
cd tinker
cd fftw
./configure --prefix=/path_to_tinkerfolder/fftw/ --enable-openmp --enable-threads
make -j 8
make install
cd ..
cp ./make/Makefile ./source
cd source
```
* Open Makefile and comment out default operating system (MAC, unless you have mac)
* Uncomment the default linux installation lines
* Keep the RENAME line commented out
```
make -j 8
make install

