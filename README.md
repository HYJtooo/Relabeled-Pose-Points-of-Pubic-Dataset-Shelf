# Relabeled-Pose-Points-of-Pubic-Dataset-Shelf
We relabel pedestrians' pose points in  1500 frames of 5 cameras of dataset Shelf, using the 24 human body postures of the SMPL model.

## Posture Points
The distribution of attitude points is shown in Figure.

![pic](https://github.com/HYJtooo/Target/blob/main/points.svg)

## Pose Points Storage Sequence
In `data_init.npz`, each pedestrian's pose points are stored in the following order:       
O_Joints = [15,16,20,14,17,21,13,18,22,12,19,23,1,10,11,0,5,6,4,7,3,8,2,9]

## Pose Point Connection
Connect the pose points in the following order:            
smpl_connection = [ [0,1],[0,2],[0,3],[1,4],[4,7],[7,10],[2,5],[5,8],[8,11],[3,6],[6,9],[9,13],
                    [9,14],[13,16],[16,18],[18,20],[20,22],[14,17],[17,19],[19,21],[21,23],
                    [9,12],[12,15]  ]

## Using
Download `data_init.npz`     
Save `data_init.npz`         
Read data in `frame-camera-person-points` order


