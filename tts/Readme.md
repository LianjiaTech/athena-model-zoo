# Data_Baker Fastspeech2 model

These models are trained on [data_baker]("https://weixinxcxdb.oss-cn-beijing.aliyuncs.com/gwYinPinKu/BZNSYP.rar")
## Inference

### python Inference with saved model



```
cd tts/data_baker/saved_model
tar -xf fastspech2.tar
$ python athena/inference.py tts/data_baker/fastspeech2_test.json
```


If you want to used the saved model to do decoding you can write the decode json file like this  
```jsonc
"saved_model_dir": "examples/tts/data_baker/saved_model/fastspeech2",
```
If you don't want to use this function you can changed your decode json file like: 
```jsonc
"saved_model_dir": null,
```