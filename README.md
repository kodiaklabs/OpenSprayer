# OpenSprayer

Here we collaborate with [Open Sprayer](http://www.opensprayer.com/) to help construct the image recognition algorithm for a land-based autonomous crop spraying drone. We take provided tagged images or weeds and non-weeds, and use CNNs to produce an image classifier via the [FastAI](fast.ai) library (PyTorch backend).

In more detail, we use a pre-trained ResNet34 architecture, for which we transfer learn on our data set. We apply multiple, small techniques such as cyclical learning rates, increasing image sizes, and un/freezing grouped layers to produce an accurate classifier.
