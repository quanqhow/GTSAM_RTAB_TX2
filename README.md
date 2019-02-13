# GTSAM_RTAB_TX2
GTSAM_RTAB_TX2


cd gtsam

Set cmake variable GTSAM_USE_SYSTEM_EIGEN=ON -->Add set(GTSAM_USE_SYSTEM_EIGEN ON) in cmakelists.txt
mkdir build && cd build
cmake ..
sudo make install

kalibr_calibrate_cameras --target april_6x6_50x50cm_8.yaml --bag intel123_2019-02-13-16-42-31.bag --bag-from-to 7 120 --models pinhole-radtan pinhole-radtan --topics /camera/infra1/image_rect_raw /camera/infra2/image_rect_raw 
