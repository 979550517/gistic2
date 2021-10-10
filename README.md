# gistic2
gistic2下载及安装
mkdir GISTIC2
mv GISTIC_2_0_23.tar.gz GISTIC2/ && cd GISTIC2/
tar zxf GISTIC_2_0_23.tar.gz
mkdir MATLAB_Compiler_Runtime
cd MCR_Installer/
unzip MCRInstaller.zip 
./install -mode silent -agreeToLicense yes -destinationFolder ~/biosoft/GISTIC2/MATLAB_Compiler_Runtime/
export LD_LIBRARY_PATH=/home/user/software/gistic2/matlab/v83/runtime/glnxa64:/home/user/software/gistic2/matlab/v83/bin/glnxa64:/home/user/software/gistic2/matlab/v83/sys/os/glnxa64:$LD_LIBRARY_PATH
export XAPPLRESDIR=/home/user/software/gistic2/matlab/v83/X11/app-defaults:$XAPPLRESDIR
export PATH=$PATH:$LD_LIBRARY_PATH
export PATH=$PATH:$XAPPLRESDIR
