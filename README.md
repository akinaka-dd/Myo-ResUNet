# ResNet50-UNet

## Preprocessing
<div align="center">
  <table>
    <tr>
      <td><img src="img/Prep/TEM01-00_01.png" width="200px"></td>
      <td><img src="img/Prep/TEM01-00_gray_cont_01.png" width="200px"></td>
      <td><img src="img/Prep/TEM01-00_rotated_gray_cont_01.png" width="200px"></td>
      <td><img src="img/Prep/TEM01-00_rotated_gray_crop_01.png" width="200px"></td>
      <td><img src="img/Prep/TEM01-00_rotated_gray_mask_crop_01.png" width="200px"></td>
    </tr>
    <tr>
      <td>A</td>
      <td>B</td>
      <td>C</td>
      <td>D</td>
      <td>E</td>
    </tr>
  </table>
</div>

## Sampling

<img src="img/Crop/C00.png" width="400px">

## Training

### Data augmentation

### Softmax

### Improvement of accuracy
<div align="center">
  <img src="img/TEM01-00_FT-resnet50-AdamW_accuracy.png" width="600px">
</div>

### Grad-CAM

<div align="center">
  <table>
    <tr>
      <td><img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval.png" width="200px"></td>
      <td><img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_p.png" width="200px"></td>
      <td><img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_cam.png" width="200px"></td>
      <td><img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_cam_bl.png" width="200px"></td>
      <td><img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_sp.png" width="200px"></td>
      <td><img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_sp_bl.png" width="200px"></td>
    </tr>
    <tr>
      <td>A</td>
      <td>B</td>
      <td>C</td>
      <td>D</td>
      <td>E</td>
      <td>F</td>
    </tr>
  </table>
</div>


