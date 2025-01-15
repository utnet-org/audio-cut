# 在线音频切割器
**https://vocalremover.org/zh/cutter**

## 1. 录音(要有麦克风)， 或者手机打开网站开启
**https://vocalremover.org/zh/voice-recorder**

![在线录音](./fixture/1.png)

## 2. 保存并且编辑

![编辑录音](./fixture/2.png)

## 3. 裁剪音频片段, 1 -3 个 30s 片段
![裁剪录音](./fixture/3.png)

## 4. 保留人声, 干音

![保留人声](./fixture/4.png)

## 5. 码率转换
![采样率](./fixture/5.png)
https://www.audio2edit.com/zh/convert-from-audio
## 6. 最后用处理过的1-3个 10s 内的wav文件就好
clone a voice submit the filename of a wave file containing the source voice

voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~5-30 sec) sample of the target speaker's voice. The sample should be a clean recording with no background noise or music.

**即时模式**

1. 录音器按照0.8的正常语速，保持样本时长在10-30秒左右，更长并不一定更好。

2. 确保音频已降采样为单声道、22050Hz、16位WAV文件。否则，会大幅降低处理速度，并且可能导致质量问题（根据几次测试结果）。输出质量本身是24000Hz！

3. 使用最新版本的Audacity，选择你的音频片段，然后选择 Tracks > Resample，设置为22050Hz，再选择 Tracks > Mix > Stereo to Mono，然后 File > Export Audio，将其保存为22050Hz的WAV文件。

如果需要进行音频清理，请确保在将音频压缩为上述设置（单声道、22050Hz、16位）之前完成。

4. 确保使用的片段没有背景噪音或音乐。例如，许多电影中的对白部分会有轻微的背景音乐。低质量音频可能会有嗡嗡声，需要清除。即使我们听不见，AI也能感知到这些噪音，并在一定程度上将其应用于模拟的声音中，所以干净的音频非常重要！

5. 尽量让你的片段是流畅的语音，像示例文件中的那样。避免有太多的停顿、间隙或其他声音。最好选择一个讲述者语音有一定起伏的片段。

确保片段不以呼吸声开始或结束（例如吸气/呼气等）。

使用AI生成的音频片段可能会引入不必要的声音，因为它本身就是对声音的复制/模拟。不过，这点需要通过测试来确认。

**专业克隆模式**

AIE的专业语音克隆功能可以创建一个高度匹配您自身声音的AI版本，几乎是完美的复制品。与即时语音克隆相比，AIE的专业语音克隆具有独特的优势。它可以对您提供的语音数据进行精细训练，生成一个几乎无法与原始声音区分的高保真语音模型。

专业克隆的模型训练过程需要一定的时间，具体时间因多种因素而异。通常，预计需要2到5分钟，这比市场上其他类似产品要显著更短。我们始终致力于为用户提供高效优质的服务，以确保您能够以最快的速度获得高质量的语音克隆结果。

🎙️ **专业录音设备**：为了达到最佳效果，强烈建议使用高质量的录音设备。高质量的音频输入将带来出色的输出质量。可以尝试各种麦克风，但连接到专用音频接口的XLR麦克风效果更佳。例如，连接到类似Focusrite的音频接口的Audio-Technica AT2020或Rode NT1可以为您的录音提供更高的保障。

🗣️ **使用防喷网**：在录音过程中，一定要使用防喷网，它可以有效减少爆破音的出现，使您的音频更加清晰自然。

📏 **控制麦克风距离**：保持适当的麦克风距离至关重要。一般来说，距离麦克风约两拳的距离较为合适，但您可以根据具体的录音需求灵活调整。

🔇 **无噪音录音环境**：确保音频输入没有干扰，例如背景音乐或其他噪音。纯音频输入会大大增强克隆效果。

🎵 **房间声学优化**：最好在经过声学处理的房间中录音。如果条件不允许，也可以使用厚被子等物品来暂时改善录音环境，以减少回声和背景噪音。

⚙️ **音频预处理（可选）**：如果你追求特定的声音输出效果，可以在上传之前编辑音频。例如，如果你希望实现类似高质量播客的效果，可以预处理音频以满足相应的质量标准。如果音频中有许多停顿或插入，AI也会准确地模仿它们。

🎚️ **精确音量控制**：保持音量稳定适中，确保音频清晰可听且不因音量过高而失真。理想的均方根值应在-23dB到-18dB之间，真实峰值为-3dB。

🔊 **音频长度足够**：为了获得更好的语音克隆效果，建议提供超过3分钟的高质量音频。更多高质量的数据将带来更出色的语音克隆效果。如果需要上传更长时间的音频，可以将其分成多个1分钟的样本，以便更方便地上传。

📁 **上传注意事项**：如果上传的音频有噪音，请使用音频增强功能来减少噪音，否则克隆效果可能不好。

即时模式

录音器按照0.8的正常语速，保持样本时长在30秒左右，更长并不一定更好。
确保音频已降采样为单声道、22050Hz、16位WAV文件。否则，会大幅降低处理速度，并且可能导致质量问题（根据几次测试结果）。输出质量本身是24000Hz！
使用最新版本的Audacity，选择你的音频片段，然后选择 Tracks > Resample，设置为22050Hz，再选择 Tracks > Mix > Stereo to Mono，然后 File > Export Audio，将其保存为22050Hz的WAV文件。
如果需要进行音频清理，请确保在将音频压缩为上述设置（单声道、22050Hz、16位）之前完成。
确保使用的片段没有背景噪音或音乐。例如，许多电影中的对白部分会有轻微的背景音乐。低质量音频可能会有嗡嗡声，需要清除。即使我们听不见，AI也能感知到这些噪音，并在一定程度上将其应用于模拟的声音中，所以干净的音频非常重要！
尽量让你的片段是流畅的语音，像示例文件中的那样。避免有太多的停顿、间隙或其他声音。最好选择一个讲述者语音有一定起伏的片段。
确保片段不以呼吸声开始或结束（例如吸气/呼气等）。
使用AI生成的音频片段可能会引入不必要的声音，因为它本身就是对声音的复制/模拟。不过，这点需要通过测试来确认。

专业克隆模式
AIE的专业语音克隆功能可以创建一个高度匹配您自身声音的AI版本，几乎是完美的复制品。与即时语音克隆相比，AIE的专业语音克隆具有独特的优势。它可以对您提供的语音数据进行精细训练，生成一个几乎无法与原始声音区分的高保真语音模型。
专业克隆的模型训练过程需要一定的时间，具体时间因多种因素而异。通常，预计需要2到5分钟，这比市场上其他类似产品要显著更短。我们始终致力于为用户提供高效优质的服务，以确保您能够以最快的速度获得高质量的语音克隆结果。
🎙 专业录音设备：为了达到最佳效果，强烈建议使用高质量的录音设备。高质量的音频输入将带来出色的输出质量。可以尝试各种麦克风，但连接到专用音频接口的XLR麦克风效果更佳。例如，连接到类似Focusrite的音频接口的Audio-Technica AT2020或Rode NT1可以为您的录音提供更高的保障。
🗣 使用防喷网：在录音过程中，一定要使用防喷网，它可以有效减少爆破音的出现，使您的音频更加清晰自然。
📏 控制麦克风距离：保持适当的麦克风距离至关重要。一般来说，距离麦克风约两拳的距离较为合适，但您可以根据具体的录音需求灵活调整。
🔇 无噪音录音环境：确保音频输入没有干扰，例如背景音乐或其他噪音。纯音频输入会大大增强克隆效果。
🎵 房间声学优化：最好在经过声学处理的房间中录音。如果条件不允许，也可以使用厚被子等物品来暂时改善录音环境，以减少回声和背景噪音。
⚙ 音频预处理（可选）：如果你追求特定的声音输出效果，可以在上传之前编辑音频。例如，如果你希望实现类似高质量播客的效果，可以预处理音频以满足相应的质量标准。如果音频中有许多停顿或插入，AI也会准确地模仿它们。
🎚 精确音量控制：保持音量稳定适中，确保音频清晰可听且不因音量过高而失真。理想的均方根值应在-23dB到-18dB之间，真实峰值为-3dB。
🔊 音频长度足够：为了获得更好的语音克隆效果，建议提供超过3分钟的高质量音频。更多高质量的数据将带来更出色的语音克隆效果。如果需要上传更长时间的音频，可以将其分成多个1分钟的样本，以便更方便地上传。
📁 上传注意事项：如果上传的音频有噪音，请使用音频增强功能来减少噪音，否则克隆效果可能不好。

请务必记住，严格遵循这些指南将大大帮助您获得更高质量的语音克隆效果。我们的专业语音克隆服务将迅速为您提供高质量的语音克隆服务。
