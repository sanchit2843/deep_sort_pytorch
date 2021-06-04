# Deep Sort with PyTorch
The code is borrowed from https://github.com/ZQPei/deep_sort_pytorch. 

# Changes
Deep sort will return [x1, y1, x2, y2, track_id, final_class, track_id_updated] instead of [x1, y1, x2, y2, track_id] and expects number of classes as input. Here "final_class" is the class with maximum number of occurances for all the frames for which specific object is tracked(change line 69 in deep_sort/deep_sort.py to change this strategy.). Unique track_id for each object is changed to per class id stored in variabl "track_id_updated", thus the counter for each class will be initialized from 0. 
