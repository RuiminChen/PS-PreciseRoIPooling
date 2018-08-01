# Position sensitive PreciseRoIPooling
I implement Position sensitive PreciseRoIPooling (Caffe ver.) based on https://github.com/vacancy/PreciseRoIPooling
 
After training PS-PreciseRoIPooling based light-head rcnn model for 20000 iterations， I got a not bad result.

I do not have enough time making experiments on PASCAL VOC or COCO, If you got better results than PSRoi-align or PSRoi-pooling. Please let me know, thank you.

![sample](https://github.com/RuiminChen/PS-PreciseRoIPooling/blob/master/1.png)

## Usage

```
optional PSPRROIPoolingParameter psprroi_pooling_param = 164;
```
```
message PSPRROIPoolingParameter {
  required float spatial_scale = 1; 
  required int32 output_dim = 2; // output channel number
  required int32 group_size = 3; // number of groups to encode position-sensitive score maps
}
```
