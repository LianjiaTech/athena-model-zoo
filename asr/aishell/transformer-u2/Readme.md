# Aishell model

These models are trained on AISHELL dataset (http://www.openslr.org/33/)

## Decode

### python decode with saved model



```
cd asr/aishell/transformer-u2 
tar -xf saved_model.20220421.tar
$ python athena/decode_main.py examples/asr/$dataset_name/configs/mtl_transformer_u2_sp_fbank80_saved_model_decode.json
```


If you want to used the saved model to do decoding you can write the decode json file like this  
```jsonc
"saved_model_dir": "examples/asr/aishell/saved_model",
```
If you don't want to use this function you can changed your decode json file like: 
```jsonc
"saved_model_dir": null,
```
There is more detail in the example json file 
mtl_transformer_u2_sp_fbank80_saved_model_decode.json