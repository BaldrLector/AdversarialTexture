# AdversarialTexture
Adversarial Texture Optimization from RGB-D Scans (CVPR 2020).

![AdversarialTexture Teaser](https://github.com/hjwdzh/AdversarialTexture/raw/master/res/teaser.png)

### Scanning Data Download
Please refer to [**data**](https://github.com/hjwdzh/AdversarialTexture/raw/master/data/) directory for details.

Before run following scripts, please modify the data_path in src/config.py as the absolute path of the data folder (e.g. Adversarial/data) where you download all data.

### Prepare for Training (Optimization)
Please refer to [**src/preprocessing**](https://github.com/hjwdzh/AdversarialTexture/raw/master/src/preprocessing) directory for details.

### Run Training (Optimization)
Consider execute run_all.sh in parallel.
```
cd src/textureoptim
python gen_script.py
sh run_all.sh
```

### Result Visualization
The result will be stored in data/result/chairID/chairID.png. You can use them to replace the corresponding default texture in data/shape, and use meshlab to open obj files to see the results.

Alternatively, we provide a simple script to render results. You will be able to see the rendering comparison in data/visual.
```
cd src
python visualize.py
```
