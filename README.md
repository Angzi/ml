# ml
机器学习笔记

* 神经网络算法可视化学习资料 （visuals-first explanation）
    *  Youtube Videos by [3Blue1Brown](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)
        *  此外，还有很多很不错的[与数学有关的直观可视化内容](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
* [Interactive Explanation of Backprop](https://xnought.github.io/backprop-explainer/)
* [TensorFlow Playground](https://playground.tensorflow.org/)
* 概念
    * AP - Average Precision
    * mAP - mean Average Precision
    * [IoUTP（Jaccard Index）\FP\FN](https://learnopencv.com/intersection-over-union-iou-in-object-detection-and-segmentation/)
        * https://learnopencv.com/mean-average-precision-map-object-detection-model-evaluation-metric/   
        * True Positive (TP) — Correct detection made by the model.
        * False Positive (FP) — Incorrect detection made by the detector.
        * False Negative (FN) — A Ground-truth missed (not detected) by the object detector.
        * True Negative (TN) —This is the background region correctly not detected by the model. This metric is not used in object detection because such regions are not explicitly annotated when preparing the annotations.
        * Positive表示检测器给出了判定box（它认为这是xxxx）， Negative表示检测器没有给出判定box（它未把区域识别为xxxx）
        * True表示检测器的判定是正确的，False表示检测器的判定是错误的
        * 因此，TP表示检测器认为box里是xxx，而且这一判定是正确的（IoU大于阈值）
        * FP表示检测器认为box里是xxxx，但这一判定是错误的（要么类别搞错了，要么IoU不够大）
        * FN表示检测器没有作出判定，但实际上这一区域是存在目标的
        * TN表示检测器没有作出判定，而这一区域也确实不存在目标（是背景）
     
* Paper
    * [YoloV1](https://paperswithcode.com/method/yolov1#:~:text=YOLOv1%20is%20a%20single%2Dstage,boxes%20and%20associated%20class%20probabilities.) 
