### 


Ruilin Wang et al. 


> The complete source code of this paper can be obtained from the zip file
> For more details about the used datasets, please read the original paper.

****

### Requirements

The packages/versions we used in developing this project are all listed in the file (requirements.txt)

****

### Dataset prepare

Please download ImageNet or COCO datasets, and push them into `datasets` folder like this : 

```
├── datasets
│   ├── train
│   │   ├── xxx.jpg
│   │   ├── ...
│   ├── test
│   │   ├── xxx.jpg
│   │   ├── ...
│   ├── validation
│   │   ├── xxx.jpg
│   │   ├── ...
├── ...
├── results
```

### Pretrained Models, Models of other methods
Please download the different models from this link: 
https://pan.baidu.com/s/1Auzpk0Ol2Mx4SShRStlD8Q?pwd=ingj

our models:
Please place the model (model_checkpoint_00388.pth) in path:
/results/OK-Robustness_Batch8_Fusion_forwardTrue_backwardTrue_HflossTrue_Combined([Identity(), Jpeg_PRIS(90), JpegMask(90), Jpeg(90)])/models/

Please place the model (model_checkpoint_00342.pth) in path: 
/results/Robustness_Batch8_Fusion_forwardTrue_backwardTrue_HflossTrue_Combined([Identity(), Jpeg_PRIS(90), JpegMask(90), Jpeg(90), GN(0.001)])/models/
please 

IMN model:
Please place the model (model11) in path:
/other_method/IMN_main/model/

IMN model:
Please place the model (model_141_fmmrdb_best.pth) in path:
/other_method/GenRAN_main/RFHN/model/test_model
****


### Train

Change the settings in json file `train_settings.json`, then run the code (train.py).

The logging file and results will be saved at `results/xxx/`

### Test

Change the settings in json file `test_settings.json`, then run the code (test.py or test_introduce.py).

Note that after placing according to the model path mentioned above, the code (test_introduce.py) can be run directly to obtain the results!
The logging file and results will be saved at `results/xxx/`



### Citation

Please cite our paper if you find this repo useful!

Contact: [ruilinwang@mail.sdu.edu.cn](mailto:ruilinwang@mail.sdu.edu.cn)

