个性化语音合成文献综述
=================================================

下面摘自文献[5]

个性化语音合成的研究现状

在主流的语音合成技术中，目前音质最好的是基于大语料库的拼接合成技术。这类技术直接从原始录音中挑选最佳单元[5]，使得音质非常接近人类发声。但是，为优化音库，通常需要录制目标说话人数小时甚至数十小时的语音数据，并进行标注和切分。这在诸如公交报站、语音播报等特定说话人领域的应用中是可以接受的。然而在个性化语音合成的应用场合，可用数据很少，造成任意文本的合成音质差、自然度低。而且，拼接合成技术难以变换音色，无法在个性化语音合成中应用。基于HMM的统计参数化语音合成算法的优点是可以借助于高性能的语音信号分析与重构技术和机器学习技术，使用少量的自然语音调整声学模型，实现个性化的语音合成。

在参数化语音合成技术中，语音信号由声学参数生成。常用的声学模型，即源-滤波器模型中，声道表示为一个或一组滤波器[8]，如线性预测（Linear Prediction Coefficient，LPC）滤波器和梅尔对数谱近似（Mel Log Spectral Approximation，MLSA）滤波器等[9]，由频谱特征参数描述。激励源由基音频率（Fundamental Frequency，F0）描述。以此为基础，个性化语音生成技术可以分成两类：声音转换（Voice Conversion，VC）和说话人自适应（Speaker Adaptation，SA）[7]。VC是将合成的声学参数使用转换函数进行转换，得到目标说话人的声学参数，再合成出目标说话人的语音[10]。说话人自适应技术是非目标说话人的声学模型（Acoustic Model，AM）转换为目标说话人的声学模型，再使用参数语音合成技术实现目标说话人语音合成[11]。两种方法中的转换函数都可以通过少量目标说话人的语音得到。

综上所述，基于HMM的语音合成技术（HMM-based speech synthesis， HSS）在个性化语音合成方面具有优势。