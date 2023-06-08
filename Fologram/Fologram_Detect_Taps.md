 - In order to detect if the user moved or not an object and the initial position of this object we can use the Rec component and the pointers component to cast a ray between the tap and the spheres and get the object as it was clicked.
- I think I also notice that the update of the positions has to happen on the release stage

![IMG_ 20230601104142](IMG_20230601104142.png)

I was able to more or less make it work but it's very unstable
Added a q about this in the fologram forum: https://community.fologram.com/t/direct-manipulation-flow-in-grashopper-triggers-recursive-loop/1079/12?u=amcard 

https://photos.google.com/u/1/photo/AF1QipNpVoPOehiSwpGiqIAxxZAdjCMHtYT0WfCKX-vu 
![IMG_20230601163830](IMG_20230601163830.png)

Joyce made a solution that did not require to detect the tap start and end because apparently global variables do update  after a code modification. I think the only time they don't auto-upate is with the sync object

https://github.com/anuzk13/GrashopperFologramClay/commit/2987c2f8a838922f00630efcc2c332585c3f49fe 