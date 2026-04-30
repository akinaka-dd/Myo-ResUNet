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
<div align="center">
  <table>
    <tr>    
      <td>C00</td>
      <td><img src="img/Crop/C00.png" width="400px"></td>
    </tr>
    <tr>  
      <td>C02</td>
      <td><img src="img/Crop/C02.png" width="400px"></td>
    </tr>
    <tr>
      <td>C04</td>
      <td><img src="img/Crop/C04.png" width="400px"></td>
    </tr>
    <tr>
      <td>C06</td>
      <td><img src="img/Crop/C06.png" width="400px"></td>
    </tr>
    <tr>
      <td>C08</td>
      <td><img src="img/Crop/C08.png" width="400px"></td>
    </tr>
    <tr>
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
    </tr>
    <tr> 
      <td>C19</td>
      <td><img src="img/Crop/C19.png" width="400px"></td>
    </tr>
  </table>
</div>

  


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
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_p.png" 
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_cam.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_cam_bl.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_sp.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Grad-CAM/TEM01-00_rotated_gray_crop_C04-0024-526-1436-559-1469-34-34_FT_eval_sp_bl.png"
             style="max-width:100%; max-height:100%;">
      </td>      
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

## WSI prediction

### TEM01-00
<div align="center">
  <table>
    <tr>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_gray_rr_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_grid_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_rect_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_accu_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_fcn_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
    </tr>
    <tr>
      <td>Grayscale</td>
      <td>Pixel-wise</td>
      <td>Nearest neighbor interpolation</td>
      <td>Softmax aggregation</td>
      <td>ResNet50-UNet</td>
    </tr>
  </table>
</div>

#### Zoom in
<div align="center">
  <table>
    <tr>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_gray_04-04.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_grid_04-04.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_rect_04-04.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_accu_04-04.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM01-00/TEM01-00_rotated_gray_crop_predict_fcn_04-04.png"
             style="max-width:100%; max-height:100%;">
      </td>
    </tr>
    <tr>
      <td>Grayscale</td>
      <td>Pixel-wise</td>
      <td>Nearest neighbor interpolation</td>
      <td>Softmax aggregation</td>
      <td>ResNet50-UNet</td>
    </tr>
  </table>
</div>

### TEM07-00
<div align="center">
  <table>
    <tr>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM07-00/TEM07-00_rotated_gray_crop_gray_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM07-00/TEM07-00_rotated_gray_crop_predict_grid_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM07-00/TEM07-00_rotated_gray_crop_predict_rect_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM07-00/TEM07-00_rotated_gray_crop_predict_accu_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
      <td style="width:200px; height:200px; text-align:center;">
        <img src="img/Pred/TEM07-00/TEM07-00_rotated_gray_crop_predict_fcn_01.png"
             style="max-width:100%; max-height:100%;">
      </td>
    </tr>
    <tr>
      <td>Grayscale</td>
      <td>Pixel-wise</td>
      <td>Nearest neighbor interpolation</td>
      <td>Softmax aggregation</td>
      <td>ResNet50-UNet</td>
    </tr>
  </table>
</div>




