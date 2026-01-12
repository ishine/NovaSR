# NovaSR44
NovaSR: A fast, tiny, and high-quality neural audio upsampler.


```
from NovaSR import FastSR

upsampler = FastSR() ## downloads from huggingface
```

```
from IPython.display import Audio
lowres_audio = upsampler.load_audio('audio_path.wav')
highres_audio = upsampler.infer(lowres_audio).cpu()

display(Audio(highres_audio, rate=48000))


