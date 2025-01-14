---
mediawiki: Stochastic_Denoise
title: Stochastic Denoise
categories: [Tutorials]
name: Stochastic Denoise
dev-status: Unreleased
support-status: Unreleased
---

{% capture maintainer%}
{% include person id='funkey' %}
{% endcapture %}

{% capture source%}
{% include github org='fiji' repo='Stochastic_Denoise' %}
{% endcapture %}
{% include info-box software='ImageJ' name='Stochastic Denoise' maintainer=maintainer author='Jan Funke' source=source status='unreleased' category='[Plugins](/plugin-index)' %}The Stochastic Denoise plugin implements a current state of the art denoising algorithm. It is based on random walks through the image along paths of similar pixels, as proposed by Francisco Estrada et al. (http://www.cs.utoronto.ca/\~strider/Denoise/). If you intend to use this plugin in a publication, please cite:

Francisco Estrada, David Fleet, Allan Jepson, <b>Stochastic Image Denoising</b>, British Mashine Vision Conference 2009

## Settings

The plugin provides two parameters: The noise standard deviation <b>sigma</b> and the number of <b>samples</b> per pixel.

With the sigma setting, you can adjust the expected amount of noise in the image. The higher you choose this value, the blurrier the result will be.

To get more pleasing results, you can increase the number of samples (i.e., the number of random walks) per pixel. However, this will result in longer runtime.

![](/media/plugins/asd-1.jpg)

## Tutorial

![](/media/plugins/lena-small.jpg) ![](/media/plugins/denoised-lena-small.jpg)

Open the image you would like to denoise and start the plugin. Try the default settings first and click "Denoise". After some seconds, the denoised image will pop up. You can change the settings and retry - the denoised image will get updated.

 
