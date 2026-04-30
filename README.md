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
<!--
<div align="center">
  <table>
    <tr>    
      <td>C00</td>
      <td><img src="img/Crop/C00.png" width="400px"></td>
      <td>C02</td>
      <td><img src="img/Crop/C02.png" width="400px"></td>
    </tr>
    <tr>
      <td>C04</td>
      <td><img src="img/Crop/C04.png" width="400px"></td>
      <td>C06</td>
      <td><img src="img/Crop/C06.png" width="400px"></td>
    </tr>
    <tr>
      <td>C08</td>
      <td><img src="img/Crop/C08.png" width="400px"></td>
      <td>C10</td>
      <td><img src="img/Crop/C10.png" width="400px"></td>
    </tr>    
    <tr>
      <td>C15</td>
      <td><img src="img/Crop/C15.png" width="400px"></td>    
    </tr>
    <tr>
      <td>C18</td>
      <td><img src="img/Crop/C18.png" width="400px"></td>
      <td>C19</td>
      <td><img src="img/Crop/C19.png" width="400px"></td>
    </tr>
  </table>
</div>
-->
    
- **C00**  
<img src="img/Crop/C00.png" width="600px">
<img src="img/Crop/C02.png" width="600px">
<img src="img/Crop/C04.png" width="600px">
<img src="img/Crop/C06.png" width="600px">
<img src="img/Crop/C08.png" width="600px">
<img src="img/Crop/C10.png" width="600px">
<img src="img/Crop/C15.png" width="600px">
<img src="img/Crop/C18.png" width="600px">
<img src="img/Crop/C19.png" width="600px">


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


