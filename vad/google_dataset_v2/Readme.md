# Google_dataset_v2 model

These models are trained on Google Speech Commands Dataset V2(http://download.tensorflow.org/data/speech_commands_v0.02.tar.gz) and openslr-28 dataset (https://www.openslr.org/resources/28/rirs_noises.zip).

## Inference

### python inference with checkpoint of DNN model 

```
cd vad/google_dataset_v2/dnn 
tar -xf ckpt.tar
$ python athena/inference.py vad/$dataset_name/dnn/vad_dnn.json
```

### python infernece with checkpoint of MarbleNet model

```
cd vad/google_dataset_v2/marblenet 
tar -xf ckpt.tar
$ python athena/inference.py vad/$dataset_name/marblenet/vad_marbleNet.json
```

If you want to used other checkpoints to performance inference, you can change the json file like: 
```jsonc
"ckpt": "examples/vad/$dataset_name/dnn/ckpt",
```

There is more detail in json files specified in this example.
