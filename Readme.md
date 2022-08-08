# Athena model zoo

Utilities managing the pretrained models created by Athena(v2.0)

## Download method

```shell
git lfs clone git@git.lianjia.com:speech_tech/athena-group/athena-model-zoo.git
```


## Results

### ASR

Language  | Model Name | Training Data | Hours of Speech |   Saved model | Chunk size | Error Rate
:-----------: | :------------: | :----------: |  -------: | -------: | -------: | -------:
Chinese  | Transformer-U2 | [AISHELL Dataset](http://www.openslr.org/33/) | 178 h | asr/aishell/transformer-u2 | Full | 6.62% (CER)

### TTS

Language  | Model Name | Training Data |  Saved model 
:-----------: | :------------: | :----------: |  -------: 
Chinese  | Fastspeech2 | data_baker | tts/data_baker/saved_model/ 

### VAD

Task | Model Name |      Training Data      | Input Segment | Frame Error Rate
:-----------: | :------: | :------------: | :-----: | :----------:
VAD  | DNN | [Google Speech Commands Dataset V2](http://download.tensorflow.org/data/speech_commands_v0.02.tar.gz) | 0.21s | 8.49%
VAD  | MarbleNet | [Google Speech Commands Dataset V2](http://download.tensorflow.org/data/speech_commands_v0.02.tar.gz) | 0.63s | 2.50%
