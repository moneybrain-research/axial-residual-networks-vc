---
layout: default
---

# Abstract 

We propose a novel architecture and improved training objectives for non-parallel voice conversion. Our proposed CycleGAN-based model performs a shape-preserving transformation directly on a high frequency-resolution magnitude spectrogram, converting its style (i.e. speaker identity) while preserving the speech content. Throughout the entire conversion process, the model does not resort to compressed intermediate representations of any sort (e.g. mel spectrogram, low resolution spectrogram, decomposed network feature). We propose an efficient axial residual block architecture to support this expensive procedure and various modifications to the CycleGAN losses to stabilize the training process. We demonstrate via experiments that our proposed model outperforms Scyclone and shows a comparable or better performance to that of CycleGAN-VC2 even without employing a neural vocoder.


# Audio Samples 

**Note**: Please refer to the [paper](https://arxiv.org/abs/2102.08075) for experimental details. 



## VCTK dataset (English)

**Source** is the source speech samples. 
**Target** is the target speech samples. 
They are provided as references. Note that we did not use these data during training.


| | Source | Target | Scyclone | CycleGAN-VC2 | Ours | 
|:-|:-------|:-------|:---------|:-------------|:-----|
|<center>Female -> Female<br>(p299, p301)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p299_to_p301/gt_src/p299_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p299_to_p301/gt_tgt/p301_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p299_to_p301/scy/AB_0.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p299_to_p301/vc2/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p299_to_p301/ours/001.wav" controls preload="auto">|
|<center>Female -> Female<br>(p301, p299)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p301_to_p299/gt_src/p301_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p301_to_p299/gt_tgt/p299_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p301_to_p299/scy/BA_0.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p301_to_p299/vc2/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_p301_to_p299/ours/001.wav" controls preload="auto">|
|<center>Female -> Male<br>(p299, p311)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p299_to_p311/gt_src/p299_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p299_to_p311/gt_tgt/p311_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p299_to_p311/scy/AB_0.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p299_to_p311/vc2/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p299_to_p311/ours/001.wav" controls preload="auto">|
|<center>Male -> Female<br>(p311, p299)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p311_to_p299/gt_src/p311_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p311_to_p299/gt_tgt/p299_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p311_to_p299/scy/BA_0.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p311_to_p299/vc2/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/fm_p311_to_p299/ours/001.wav" controls preload="auto">|
|<center>Male -> Male<br>(p311, p360)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p311_to_p360/gt_src/p311_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p311_to_p360/gt_tgt/p360_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p311_to_p360/scy/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p311_to_p360/vc2/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p311_to_p360/ours/001.wav" controls preload="auto">|
|<center>Male -> Male<br>(p360, p311)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p360_to_p311/gt_src/p360_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p360_to_p311/gt_tgt/p311_001_mic1.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p360_to_p311/scy/BA_0.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p360_to_p311/vc2/001.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/mm_p360_to_p311/ours/001.wav" controls preload="auto">|


## KSS & Internal dataset (Korean)

**Target** is omitted since KSS and our internal datset are non-parallel.


|  | Source | Scyclone | CycleGAN-VC2 | Ours | 
|:-|:-------|:---------|:-------------|:-----|
|<center>Female -> Female<br>(JEY, KSS)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/gt_src/100.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/scy/KSS_00.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/vc2/KSS_00.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/ours/KSS_00.wav" controls preload="auto">|
|<center>&nbsp;<br>&nbsp;</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/gt_src/107.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/scy/KSS_07.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/vc2/KSS_07.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_JEY_to_KSS/ours/KSS_07.wav" controls preload="auto">|
|<center>Female -> Female<br>(KSS, JEY)</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/gt_src/KSS_00.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/scy/JEY_00.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/vc2/JEY_00.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/ours/JEY_00.wav" controls preload="auto">|
|<center>&nbsp;<br>&nbsp;</center>|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/gt_src/KSS_09.wav" controls="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/scy/JEY_09.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/vc2/JEY_09.wav" controls preload="auto">|<audio src="https://raw.githubusercontent.com/moneybrain-research/axial-residual-networks-vc/master/assets/audio/ff_KSS_to_JEY/ours/JEY_09.wav" controls preload="auto">|


# Citation 

```plain
@misc{you2021axial,
      title={Axial Residual Networks for CycleGAN-based Voice Conversion},
      author={Jaeseong You and Gyuhyeon Nam and Dalhyun Kim and Gyeongsu Chae},
      year={2021},
      eprint={2102.08075},
      archivePrefix={arXiv},
      primaryClass={eess.AS}
}
```
