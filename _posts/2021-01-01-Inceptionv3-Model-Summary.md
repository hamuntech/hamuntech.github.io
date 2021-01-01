---
layout: post
title: Inception v3 Model Summary
---
This is a reference post for the Google ImageNet Inception v3 model, to function as a handy reference for layer selection.

Further info about the model can be found here:

[Inceptionv3](https://en.wikipedia.org/wiki/Inceptionv3)

[Advanced Guide to Inception v3 on Cloud TPU](https://cloud.google.com/tpu/docs/inception-v3-advanced)

[Keras InceptionV3](https://keras.io/api/applications/inceptionv3/)

<table border=0 cellpadding=0 cellspacing=0 width=904 style='border-collapse:
 collapse;table-layout:fixed;width:678pt'>
 <col width=364 style='mso-width-source:userset;mso-width-alt:11648;width:273pt'>
 <col width=188 style='mso-width-source:userset;mso-width-alt:6016;width:141pt'>
 <col width=81 style='mso-width-source:userset;mso-width-alt:2602;width:61pt'>
 <col width=271 style='mso-width-source:userset;mso-width-alt:8661;width:203pt'>
 <tr height=24 style='height:18.0pt'>
  <th height=24 class=xl65 width=364 style='height:18.0pt;width:273pt'><b>Layer
  (type)</b> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</th>
  <th width=188 style='width:141pt'><b>Output Shape</b> &nbsp; &nbsp; &nbsp; &nbsp;</th>
  <th width=81 style='width:61pt'><b>Param #</b> &nbsp;</th>
  <th width=271 style='width:203pt'>&nbsp; <b>Connected to</b> &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</th>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>input_2 (InputLayer)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>[(None, 150, 150, 3)</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_94 (Conv2D)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 74, 74, 32) &nbsp;</td>
  <td>864 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; input_2[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_94
  (BatchNo</td>
  <td>(None, 74, 74, 32) &nbsp;</td>
  <td>96&nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_94[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_94
  (Activation)&nbsp; &nbsp; &nbsp;</td>
  <td>(None, 74, 74, 32) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_94[0][0]&nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_95 (Conv2D)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 72, 72, 32) &nbsp;</td>
  <td>9216&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_94[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_95
  (BatchNo</td>
  <td>(None, 72, 72, 32) &nbsp;</td>
  <td>96&nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_95[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_95
  (Activation)&nbsp; &nbsp; &nbsp;</td>
  <td>(None, 72, 72, 32) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_95[0][0]&nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_96 (Conv2D)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 72, 72, 64) &nbsp;</td>
  <td>18432 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_95[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_96
  (BatchNo</td>
  <td>(None, 72, 72, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_96[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_96
  (Activation)&nbsp; &nbsp; &nbsp;</td>
  <td>(None, 72, 72, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_96[0][0]&nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>max_pooling2d_4
  (MaxPooling2D)&nbsp;</td>
  <td>(None, 35, 35, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_96[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_97 (Conv2D)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 35, 35, 80) &nbsp;</td>
  <td>5120&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_4[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_97
  (BatchNo</td>
  <td>(None, 35, 35, 80) &nbsp;</td>
  <td>240 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_97[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_97
  (Activation)&nbsp; &nbsp; &nbsp;</td>
  <td>(None, 35, 35, 80) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_97[0][0]&nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_98 (Conv2D)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 33, 33, 192)&nbsp;</td>
  <td>138240&nbsp; &nbsp;</td>
  <td>&nbsp; activation_97[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_98
  (BatchNo</td>
  <td>(None, 33, 33, 192)&nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_98[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_98
  (Activation)&nbsp; &nbsp; &nbsp;</td>
  <td>(None, 33, 33, 192)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_98[0][0]&nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>max_pooling2d_5
  (MaxPooling2D)&nbsp;</td>
  <td>(None, 16, 16, 192)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_98[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_102 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>12288 &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_5[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_102
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_102[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_102 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_102[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_100 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>9216&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_5[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_103 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>55296 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_102[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_100
  (BatchN</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>144 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_100[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_103
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_103[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_100 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_100[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_103 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_103[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_9
  (AveragePoo</td>
  <td>(None, 16, 16, 192)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_5[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_99 (Conv2D)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>12288 &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_5[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_101 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>76800 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_100[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_104 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>82944 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_103[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_105 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 32) &nbsp;</td>
  <td>6144&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_9[0][0] &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_99
  (BatchNo</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_99[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_101
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_101[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_104
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_104[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_105
  (BatchN</td>
  <td>(None, 16, 16, 32) &nbsp;</td>
  <td>96&nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_105[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_99
  (Activation)&nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_99[0][0]&nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_101 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_101[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_104 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_104[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_105 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 32) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_105[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed0 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 256)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_99[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_101[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_104[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_105[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_109 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>16384 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed0[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_109
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_109[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_109 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_109[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_107 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>12288 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed0[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_110 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>55296 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_109[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_107
  (BatchN</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>144 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_107[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_110
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_110[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_107 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_107[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_110 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_110[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_10
  (AveragePo</td>
  <td>(None, 16, 16, 256)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed0[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_106 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>16384 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed0[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_108 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>76800 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_107[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_111 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>82944 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_110[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_112 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>16384 &nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_10[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_106
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_106[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_108
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_108[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_111
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_111[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_112
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_112[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_106 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_106[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_108 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_108[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_111 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_111[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_112 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_112[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed1 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 288)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_106[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_108[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_111[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_112[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_116 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>18432 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed1[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_116
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_116[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_116 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_116[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_114 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>13824 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed1[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_117 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>55296 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_116[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_114
  (BatchN</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>144 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_114[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_117
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_117[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_114 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 48) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_114[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_117 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_117[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_11
  (AveragePo</td>
  <td>(None, 16, 16, 288)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed1[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_113 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>18432 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed1[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_115 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>76800 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_114[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_118 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>82944 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_117[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_119 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>18432 &nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_11[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_113
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_113[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_115
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_115[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_118
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_118[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_119
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_119[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_113 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_113[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_115 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_115[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_118 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_118[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_119 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_119[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed2 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 288)&nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_113[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_115[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_118[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_119[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_121 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>18432 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed2[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_121
  (BatchN</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>192 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_121[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_121 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 64) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_121[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_122 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>55296 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_121[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_122
  (BatchN</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_122[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_122 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 16, 16, 96) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_122[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_120 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 384)&nbsp; &nbsp;</td>
  <td>995328&nbsp; &nbsp;</td>
  <td>&nbsp; mixed2[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_123 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 96) &nbsp; &nbsp;</td>
  <td>82944 &nbsp; &nbsp;</td>
  <td>&nbsp; activation_122[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_120
  (BatchN</td>
  <td>(None, 7, 7, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_120[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_123
  (BatchN</td>
  <td>(None, 7, 7, 96) &nbsp; &nbsp;</td>
  <td>288 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_123[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_120 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_120[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_123 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 96) &nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_123[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>max_pooling2d_6
  (MaxPooling2D)&nbsp;</td>
  <td>(None, 7, 7, 288)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed2[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed3 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_120[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_123[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_6[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_128 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>98304 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed3[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_128
  (BatchN</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>384 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_128[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_128 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_128[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_129 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>114688&nbsp; &nbsp;</td>
  <td>&nbsp; activation_128[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_129
  (BatchN</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>384 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_129[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_129 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_129[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_125 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>98304 &nbsp; &nbsp;</td>
  <td>&nbsp; mixed3[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_130 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>114688&nbsp; &nbsp;</td>
  <td>&nbsp; activation_129[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_125
  (BatchN</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>384 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_125[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_130
  (BatchN</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>384 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_130[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_125 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_125[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_130 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_130[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_126 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>114688&nbsp; &nbsp;</td>
  <td>&nbsp; activation_125[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_131 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>114688&nbsp; &nbsp;</td>
  <td>&nbsp; activation_130[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_126
  (BatchN</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>384 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_126[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_131
  (BatchN</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>384 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_131[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_126 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_126[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_131 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 128)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_131[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_12
  (AveragePo</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed3[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_124 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed3[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_127 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>172032&nbsp; &nbsp;</td>
  <td>&nbsp; activation_126[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_132 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>172032&nbsp; &nbsp;</td>
  <td>&nbsp; activation_131[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_133 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_12[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_124
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_124[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_127
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_127[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_132
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_132[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_133
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_133[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_124 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_124[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_127 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_127[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_132 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_132[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_133 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_133[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed4 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_124[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_127[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_132[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_133[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_138 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>122880&nbsp; &nbsp;</td>
  <td>&nbsp; mixed4[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_138
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_138[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_138 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_138[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_139 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_138[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_139
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_139[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_139 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_139[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_135 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>122880&nbsp; &nbsp;</td>
  <td>&nbsp; mixed4[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_140 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_139[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_135
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_135[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_140
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_140[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_135 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_135[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_140 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_140[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_136 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_135[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_141 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_140[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_136
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_136[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_141
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_141[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_136 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_136[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_141 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_141[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_13
  (AveragePo</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed4[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_134 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed4[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_137 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>215040&nbsp; &nbsp;</td>
  <td>&nbsp; activation_136[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_142 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>215040&nbsp; &nbsp;</td>
  <td>&nbsp; activation_141[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_143 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_13[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_134
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_134[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_137
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_137[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_142
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_142[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_143
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_143[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_134 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_134[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_137 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_137[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_142 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_142[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_143 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_143[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed5 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_134[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_137[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_142[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_143[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_148 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>122880&nbsp; &nbsp;</td>
  <td>&nbsp; mixed5[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_148
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_148[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_148 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_148[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_149 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_148[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_149
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_149[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_149 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_149[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_145 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>122880&nbsp; &nbsp;</td>
  <td>&nbsp; mixed5[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_150 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_149[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_145
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_145[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_150
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_150[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_145 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_145[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_150 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_150[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_146 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_145[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_151 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>179200&nbsp; &nbsp;</td>
  <td>&nbsp; activation_150[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_146
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_146[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_151
  (BatchN</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>480 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_151[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_146 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_146[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_151 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 160)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_151[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_14
  (AveragePo</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed5[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_144 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed5[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_147 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>215040&nbsp; &nbsp;</td>
  <td>&nbsp; activation_146[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_152 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>215040&nbsp; &nbsp;</td>
  <td>&nbsp; activation_151[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_153 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_14[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_144
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_144[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_147
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_147[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_152
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_152[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_153
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_153[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_144 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_144[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_147 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_147[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_152 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_152[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_153 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_153[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed6 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_144[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_147[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_152[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_153[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_158 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed6[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_158
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_158[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_158 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_158[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_159 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_158[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_159
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_159[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_159 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_159[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_155 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed6[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_160 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_159[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_155
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_155[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_160
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_160[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_155 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_155[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_160 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_160[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_156 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_155[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_161 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_160[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_156
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_156[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_161
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_161[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_156 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_156[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_161 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_161[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_15
  (AveragePo</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed6[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_154 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed6[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_157 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_156[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_162 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_161[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_163 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_15[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_154
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_154[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_157
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_157[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_162
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_162[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_163
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_163[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_154 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_154[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_157 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_157[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_162 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_162[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_163 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_163[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed7 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_154[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_157[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_162[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_163[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_166 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed7[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_166
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_166[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_166 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_166[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_167 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_166[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_167
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_167[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_167 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_167[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_164 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>147456&nbsp; &nbsp;</td>
  <td>&nbsp; mixed7[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_168 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>258048&nbsp; &nbsp;</td>
  <td>&nbsp; activation_167[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_164
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_164[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_168
  (BatchN</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_168[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_164 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_164[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_168 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 7, 7, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_168[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_165 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>552960&nbsp; &nbsp;</td>
  <td>&nbsp; activation_164[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_169 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>331776&nbsp; &nbsp;</td>
  <td>&nbsp; activation_168[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_165
  (BatchN</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>960 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_165[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_169
  (BatchN</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_169[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_165 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_165[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_169 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_169[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>max_pooling2d_7
  (MaxPooling2D)&nbsp;</td>
  <td>(None, 3, 3, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed7[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed8 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 1280) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_165[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_169[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; max_pooling2d_7[0][0] &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_174 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 448)&nbsp; &nbsp;</td>
  <td>573440&nbsp; &nbsp;</td>
  <td>&nbsp; mixed8[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_174
  (BatchN</td>
  <td>(None, 3, 3, 448)&nbsp; &nbsp;</td>
  <td>1344&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_174[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_174 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 448)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_174[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_171 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>491520&nbsp; &nbsp;</td>
  <td>&nbsp; mixed8[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_175 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1548288 &nbsp;</td>
  <td>&nbsp; activation_174[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_171
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_171[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_175
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_175[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_171 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_171[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_175 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_175[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_172 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_171[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_173 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_171[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_176 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_175[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_177 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_175[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_16
  (AveragePo</td>
  <td>(None, 3, 3, 1280) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed8[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_170 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>409600&nbsp; &nbsp;</td>
  <td>&nbsp; mixed8[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_172
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_172[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_173
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_173[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_176
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_176[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_177
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_177[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_178 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>245760&nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_16[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_170
  (BatchN</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>960 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_170[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_172 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_172[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_173 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_173[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_176 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_176[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_177 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_177[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_178
  (BatchN</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_178[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_170 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_170[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed9_0 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_172[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_173[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>concatenate_2 (Concatenate)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_176[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_177[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_178 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_178[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed9 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 2048) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_170[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed9_0[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; concatenate_2[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_178[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_183 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 448)&nbsp; &nbsp;</td>
  <td>917504&nbsp; &nbsp;</td>
  <td>&nbsp; mixed9[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_183
  (BatchN</td>
  <td>(None, 3, 3, 448)&nbsp; &nbsp;</td>
  <td>1344&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_183[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_183 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 448)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_183[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_180 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>786432&nbsp; &nbsp;</td>
  <td>&nbsp; mixed9[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_184 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1548288 &nbsp;</td>
  <td>&nbsp; activation_183[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_180
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_180[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_184
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_184[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_180 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_180[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_184 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_184[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_181 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_180[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_182 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_180[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_185 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_184[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_186 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>442368&nbsp; &nbsp;</td>
  <td>&nbsp; activation_184[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>average_pooling2d_17
  (AveragePo</td>
  <td>(None, 3, 3, 2048) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed9[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_179 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>655360&nbsp; &nbsp;</td>
  <td>&nbsp; mixed9[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_181
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_181[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_182
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_182[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_185
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_185[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_186
  (BatchN</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>1152&nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_186[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>conv2d_187 (Conv2D) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>393216&nbsp; &nbsp;</td>
  <td>&nbsp; average_pooling2d_17[0][0]&nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_179
  (BatchN</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>960 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_179[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_181 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_181[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_182 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_182[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_185 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_185[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_186 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 384)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_186[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>batch_normalization_187
  (BatchN</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>576 &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; conv2d_187[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_179 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 320)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_179[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed9_1 (Concatenate)&nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_181[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_182[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>concatenate_3 (Concatenate)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 768)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_185[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_186[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>activation_187 (Activation)
  &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 192)&nbsp; &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; batch_normalization_187[0][0]</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>mixed10 (Concatenate) &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>(None, 3, 3, 2048) &nbsp;</td>
  <td>0 &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_179[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; mixed9_1[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; concatenate_3[0][0] &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>&nbsp;&nbsp; &nbsp; &nbsp;
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
  &nbsp;</td>
  <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
  <td>&nbsp; activation_187[0][0]&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>===============================</td>
  <td>======================</td>
  <td>=========</td>
  <td>================================</td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>Total params: 21,802,784</td>
  <td colspan=3 style='mso-ignore:colspan'></td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>Trainable params: 0</td>
  <td colspan=3 style='mso-ignore:colspan'></td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>Non-trainable params:
  21,802,784</td>
  <td align=right></td>
  <td colspan=2 style='mso-ignore:colspan'></td>
 </tr>
 <tr height=24 style='height:18.0pt'>
  <td height=24 class=xl65 style='height:18.0pt'>_______________________________</td>
  <td>______________________</td>
  <td>_________</td>
  <td>________________________________</td>
 </tr>
</table>