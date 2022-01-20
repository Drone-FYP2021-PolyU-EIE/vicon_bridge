# Setup
## ROS
Clone to the Ros Workspace    
```bash
git clone https://github.com/ethz-asl/vicon_bridge.git
```

### MAV ROS config
vision_pose/tf/listen (bool, default: false) set to `True`    
TF listen switch. Disable topic if enabled.   
vision_pose/tf/frame_id (string, default: local_origin) set to `/vicon/world`   
Origin frame_id for TF.   
vision_pose/tf/child_frame_id (string, default: vision) set to  UAV TF path   
Child frame_id for TF.    


## QGC
### EKK 2
`EKF2_AID_MASK` to `15`   
`EKF2_HGT_MODE` to `3`(Vision)    

if you are using USB to connect UAV   
`CBRK_USB_CHK` check if it is `197848`    
### ATT
